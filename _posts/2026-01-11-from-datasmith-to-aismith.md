---
layout: post
title: "From DataSmith to AISmith"
description: "Build more, use ai more, and be visible."
tags: [research, en]
---


Over the winter break, I have been reflecting on the strategy for our lab. Our stance in the past 3 years was simple: do the work, publish when it’s ready, keep a low profile otherwise. It was how I did my PhD, and how I recruited students—people who liked the craft more than the limelight. In retrospect, that seemed fine when prestigious academic venues still carried the signal they once did, when funding was stable, and when the range of problems was less sharply dominated by one major trend (i.e., AI).

However, that world is changing. The pace and incentives of research have shifted. AI has become a wave that reorganizes everything it touches—topics, funding, jobs. Federal support is tightening in some areas; industry is offering alternative routes that look more attractive to students than the old academic pilgrimage. Some privacy research is increasingly swimming against a tide of rapid AI innovation that lowers regulatory and institutional barriers in the name of speed [[1]](#notes). Since compliance remains the primary driver of privacy in the industry, the need for privacy research is also decreasing. In short, the landscape that made our old rules sensible is receding.

When the landscape changes, there are two obvious reactions. One is to double down on the old virtues—more discipline, more insulation, more purity. The other is to be pragmatic: identify the unique capabilities you have, and redeploy them in the directions that matter now. Neither is superior. But if the aim is to have impact and to prepare students for the world they will inhabit, pragmatism has a certain compulsive clarity.

Our lab sits at the intersection of systems, privacy/security, and HCI. That’s not an accident—it’s a sweet spot for tool-building. We can do things that pure HCI folks or pure systems researchers can’t. We should exploit that. When I started the lab, I named it the Data Smith Lab—not the Data Privacy Lab—because I’ve always loved the idea of “Computer Science as a Toolsmith”  [[2]](#notes). Over the past three years, we’ve made privacy our primary focus. Now it’s time to revisit—and strengthen—the other two pillars as well.

I see a major opportunity that aligns with our strengths: designing human-on-the-loop interaction for emerging agentic experiences. Human-in-the-loop approaches have been studied for decades under a familiar division of labor—humans handle what machines cannot, and machines take on what humans would rather not do. But we are reaching a tipping point: across many tasks, **human oversight can no longer keep pace with AI**, making people the bottleneck in human–AI teaming. Like it or not, the industry will continue to push toward agentic experiences, even if many of today’s “agent” techniques do not endure. The broader idea—*agentic interaction*, in which people delegate goals and supervision rather than issue step-by-step commands—captures a fundamental concept of how people want the world to run. However, LLM-based systems remain inherently unreliable, and increasing autonomy correspondingly increases the likelihood of failures and safety incidents. That is the bet I want to make: to build the interaction and system foundations for **safe human-on-the-loop control**, where people can set direction, audit behavior, and intervene effectively—without being forced into continuous, fragile micromanagement.

OK. So what would be the differences for the lab? Not that much.

First, build usable systems. Publishable ideas are valuable. But the conventional academic cycle—ideation, paper, long review, near-forgotten demo— was too slow. A project started now may take 12 months or more before it reaches the world, and in that time, even strong ideas can lose their relevance. Consider DeepSeek-R1, released in January 2025: if you’ve been following the field, it already feels like history. I’ll **push everyone for more time building**—call it roughly 80%—because nothing else substitutes for hands-on, iterative understanding. We will re-prioritize the steps in the research workflows. Put usable artifacts in front of people early. Write blog posts explaining the thought and findings. Show failures as well as wins. The aim is not to chase attention but to pull real feedback sooner.

Second, use AI more aggressively. **Treat AI tools like your bitcoin mining machine: if they’re idle while you sleep, you are losing money.** Have your projects serve as testbeds for agentic tools that continue to work when you go to sleep, eat, and rest. The will train you to judge an AI’s pragmatic reliability—when to trust it, when to supervise it, when to rework the pipeline to reduce its brittleness.

Third, be visible. This might be the main reason I’m writing this essay. I take an unusually broad view of privacy—nearly all safety problems can be reframed as privacy-related questions about what data is collected, inferred, retained, and acted upon. But a message is only effective if others share the same understanding. This is why I think we should rebrand as **AI Smith Lab**. “Data Smith” or “Toolsmith” still fits, but “AI Smith” makes our focus legible to the people we most need to engage.


##### Notes

[1] In response to the Executive Order on AI and America’s AI Action Plan, the FTC has set aside a final order against a company that offered an AI service enabling consumers to draft online reviews. In its press release, the FTC notes that it is focused on fraud and tangible consumer harm. [FTC Reopens and Sets Aside Rytr Final Order in Response to the Trump Administration’s AI Action Plan](https://www.ftc.gov/news-events/news/press-releases/2025/12/ftc-reopens-sets-aside-rytr-final-order-response-trump-administrations-ai-action-plan)  

[2] [Computer Science as a Toolsmith](https://www.cs.unc.edu/~brooks/Toolsmith-CACM.pdf) 
