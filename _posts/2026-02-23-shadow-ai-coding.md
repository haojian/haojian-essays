---
layout: post
title: "Shadowing How Peter Steinberger Codes with AI"
description: "AI coding is a tool rather than a lootbox. "
tags: [research, en]
---

> I spent 3 hours watching [OpenClaw's creator code](https://www.youtube.com/watch?v=68BS5GCRcBo), frame by frame. Here's what I learned about the gap between amateur and elite AI-assisted programming.

<iframe width="560" height="315" src="https://www.youtube.com/embed/68BS5GCRcBo?si=U8JnVejo6tcwLAtB" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


My first job was at Yahoo. On day one, my manager didn't give me a project. Instead, he told me to shadow a senior engineer with 20+ years of experience. I sat in the cubicle next to the senior engineer for a few hours and watched everything — every keystroke, every mouse movement, every shortcut. When I didn't understand something, I asked: Why this shortcut? Why not use the mouse here? That experience influenced my working habits for many years. 

Recently, my lab started building [AI Coding Gym](https://aicodinggym.com/), a platform to help people practice AI-assisted programming. Honestly, we're not the best AI coders ourselves. My students suggested we interview top AI coders to learn their techniques. But when I looked around, most people seemed to be doing what we were doing — prompting AI, opening multiple agents in terminals managed by a [tmux](https://github.com/tmux/tmux/wiki), trying to create an agent team, but most of them failed.

Then I came across a [livestream by Peter Steinberger from September 2025](https://www.youtube.com/embed/68BS5GCRcBo?si=U8JnVejo6tcwLAtB). Peter is the creator of [OpenClaw](https://openclaw.ai/) — back then he wasn't as famous as he is now. In the stream, he built a completely new feature for a Twitter analytics platform from scratch using OpenAI Codex. I watched the entire thing frame by frame, like I was back in that Yahoo cubicle doing my shadow engineering rotation.

His workflow had a kind of stunning elegance. Every detail made sense. I could see *why* each choice was right, but I had never noticed these details before. Here's what I took away:

—

**AI coding comes down to two things: attention and context management.**

Attention first. There's no real difference between AI coding and vibe coding. In the stream, Peter was watching every terminal, tracking what each agent was doing, correcting course constantly. He mentioned that the night before, he got tired at 2am and started vibe coding — "the shit happens." The AI agents in his hands don't have much autonomy. They're tools, not collaborators. He doesn't trust AI output. He manually verifies everything — clicks through the feature like a user before moving on. But he also lets AI yolo when his attention has to prioritize the few more important things. 

Context management second, but arguably more important. Tools will change. Models will iterate. Today's Codex might be replaced tomorrow. But the problem of "how to efficiently ship a feature within a finite context window" isn't going away anytime soon. Everything he does is in service of preserving context. He avoids MCPs because they're slow and bloat the context. He opens a fresh session (/new) for every new feature. One of his quotes was particularly interesting: when the remaining context drops below 33%, the model "gets drunk and stupid." He intentionally designed features to fit inside one context window. If they don't fit, break them down. 

<!-- Build the smallest working version first, then let the AI use that working example as a template to expand. -->

—

**Tools.** This is the easiest gap to close. I noted the tools he uses that I don't.

![alt text](/resources/ghostty.png)

Hardware: Mac desktop, Dell ultrawide monitor, 4 [Ghostty terminal](https://ghostty.org/) windows side by side. Left: Codex running database migration. Center: two agents building separate features. Right: server + terminal. More agents = more splits.

He uses [Wispr Flow](https://wisprflow.ai/) (recently acquired by Apple) for voice-to-prompt input. 

[Sublime Merge](https://www.sublimemerge.com/) for diffs. 

Use CLI (command line interface) over MCP, because it's faster and saves context. He vibe-coded many CLI tools himself. One example is Better Stack Logs, which provides a web-based interface for monitoring logs. Since they are only used in the development environment, he doesn't even read the code of these CLI tools. 

He uses many services from startups I'd never heard of before. [Linear](https://linear.app/) CLI for task management,  [Inngest](https://www.inngest.com/) for background jobs. These modern services are more compatible with AI agents. For example, [Inngest](https://www.inngest.com/) has [llms.txt files](https://www.inngest.com/llms.txt).



—

**claude.md is the AI's operating manual.** He writes code style rules, lint configurations, and detailed database instructions into a project-based Claude.md. I like the language he used: the Claude.md will "**morph the chaos it (AI) produces into a code style that I like.**" 

The database section in Claude.md is the largest — because database operations are where things go wrong the most. Keep it concise, split into multiple files if needed, and let the model help you maintain it.

![alt text](/resources/peter-db.png)

—

**Coding habits.** He doesn't use TDD (test-driven development). He prefers to let AI write the feature and have AI write the tests, then manually verifies it works. Because the AI wrote the code, it can also write the unit tests well. This conflicts with my prior understanding, but makes sense. 

He mostly works on the main branch. This might be due to the project stage. He tried worktrees, but it led to too many conflicts. He tries to only implement 1-3 features in parallel. Design tasks so agents can work on non-conflicting modules. Most of the time, he turns YOLO mode on his development machine, but with discipline: never delete, only move. He feels it's fine, especially if everything is in Git and the machine does nightly backups.

—

**His actual prompt**: the last fun part is that he combined Wispr Flow with keyboard typing when interacting with the terminals. I'm not sure if it's because he was in the middle of streaming, but it definitely seems like a more modern approach.


![alt text](/resources/prompts-peter.png)

I guess he must have practiced this many times. He casually spoke these sentences during the stream, but I found these prompts fit his principles quite well: clear feature boundary, explicit data caps (1,000 tweets distributed by user count), preprocessing requirements (text only, no metadata), output format (table), storage design (cache table). One prompt, one complete feature, sized to fit one context window.


