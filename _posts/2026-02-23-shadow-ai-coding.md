---
layout: post
title: "Shadow How Peter Steinberger Coding with AI"
description: "AI coding is context window management. Save every token you can. Verify manually. Break things down. Let AI handle the rest."
tags: [research, en]
---

> I spent 3 hours watching [OpenClaw's creator code](https://www.youtube.com/watch?v=68BS5GCRcBo), frame by frame. Here's what I learned about the gap between amateur and elite AI-assisted programming.

<iframe width="560" height="315" src="https://www.youtube.com/embed/68BS5GCRcBo?si=U8JnVejo6tcwLAtB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


My first job was at Yahoo. On day one, my manager didn't give me a project. Instead, he told me to shadow a senior engineer with 20+ years of experience for the first few days. I sat in the cubicle next to him and watched everything — every keystroke, every mouse movement, every shortcut. When I didn't understand something, I asked: why this shortcut? Why not use the mouse here?

That experience stuck with me. Recently, my lab started building [AI Coding Gym](https://aicodinggym.com/), a platform to help people practice AI-assisted programming. Honestly, we're not the best AI coders ourselves. My students suggested we interview top AI coders to learn their techniques. But when I looked around, most people seemed to be doing what we were doing — flailing around with AI, throwing punches in the dark.

Then I came across a livestream by Peter Steinberger from September 2025. Peter is the creator of OpenClaw — back then he wasn't as famous as he is now. In the stream, he built a complete new feature for a Twitter analytics platform, from scratch, using Claude Code and Codex. I watched the entire thing frame by frame, like I was back in that Yahoo cubicle doing my shadow engineering rotation.

His workflow had a kind of brutal elegance. Every detail made sense. I could see *why* each choice was right, but I had never noticed these details before. That gap — between knowing the tools exist and knowing how to orchestrate them — is probably the difference between my flailing and his OpenClaw.

Here's what I took away:

—

**AI coding comes down to two things: attention and context management.**

Attention first. There's no real difference between AI coding and vibe coding — except that when you're building serious software, vibe coding produces garbage. In the stream, Peter was watching every terminal, tracking what each agent was doing, correcting course constantly. He mentioned that the night before, he got tired at 2am and started vibe coding — "the shit happens." The AI agents in his hands don't have much autonomy. They're instruments, not collaborators. He doesn't trust AI output. He manually verifies everything — clicks through the feature like a user before moving on.

Context management second, but arguably more important. Tools will change. Models will iterate. Today's Codex might be replaced tomorrow. But the problem of "how to efficiently ship a feature within a finite context window" isn't going away anytime soon. Everything he does is in service of preserving context. He avoids MCPs because they're slow and bloat the context. He doesn't rely on automatic context compaction. He opens a fresh session (/new) for every new feature.

His rule of thumb: when the remaining context drops below 33%, the model "gets drunk and stupid." Design the features to fit inside one context window. If they don't fit, break them down. Build the smallest working version first, then let the AI use that working example as a template to expand.

—

**Tools.** For gear enthusiasts, this is the easiest gap to close.

![alt text](/resources/ghostty.png)

Hardware: Mac desktop, Dell ultrawide monitor, 4 Ghostty terminal windows side by side. Left: Codex running database migration. Center: two agents building separate features. Right: server + terminal. More agents = more splits.

He uses [Wispr Flow](https://wisprflow.ai/) (recently acquired by Apple) for voice-to-prompt input. Sublime Merge for diffs. Only one MCP — Brave search API. Everything else runs through CLI tools, many of which he vibe-coded himself. He uses Linear CLI for task management, Better Stack Logs for monitoring, Inngest for background jobs. Modern services that ship with llms.txt files so AI agents can understand how to use them out of the box.



—

**claude.md is the AI's operating manual.** He writes code style rules, lint configurations, and detailed database instructions into it. His quote: "morph the chaos it produces into a code style that I like." The database section is the largest — because database operations are where things go wrong most. Keep it concise, split into multiple files if needed, and let the model help you maintain it.

—

**Coding habits.** System design before code. Plan mode first. No TDD (test-driven development) — write the feature, manually verify it works, then have AI write the tests. Work on main branch (he tried worktrees, too many conflicts). Only 1-3 features in parallel. Design tasks so agents work on non-conflicting modules — clean commits, double the speed. YOLO mode on, but with discipline: never delete, only move. Everything in Git. Nightly backups.

—

**His actual prompt** (dictated via Wispr Flow, verbatim):



![alt text](/resources/prompts-peter.png)


Notice what makes this prompt effective: clear feature boundary, explicit data caps (1,000 tweets distributed by user count), preprocessing requirements (text only, no metadata), output format (table), storage design (cache table). One prompt, one complete feature, sized to fit one context window.


