---
draft: "true"
---

## Andrew Baker

 I led the Twilio developer education team for a while. I actually joined up as an individual contributor first.

What drew me to the team in the first place was kind of the core ethos I would say Twilio was bringing to the space, which was: the best folks to create excellent documentation for developer customers are engineers themselves, not technical writers. That really attracted me because prior to that I started my career as a Python engineer in Washington, DC, mostly in the government consulting space.

I actually got really lucky, got staffed on some really fun government clients, like the Consumer Financial Protection Bureau. Got to meet some cool technologists who rotated in through industry. That was a special experience in retrospect. But I was ready for a break and wanted to work for a product company next. 

Before I did that, I took a little time off to tinker with my own interests. That was when Docker was getting really hot for the first time, so I had the opportunity to lean into it. I built some Docker tutorials and workshops, ran them at meetups, started putting in talks at Python conferences. I'd already found my way as someone who was an engineer but just really enjoyed teaching other engineers.

So I stumbled into this sort of role. I thought, oh, I guess I should go and try to find a job doing something like this. I got lucky that around the same time Twilio was starting this developer education team—one of only a handful in the industry in 2015 supporting docs this way. Most companies were still, A) not treating the engineer as their customer persona, and B) running docs as a conventional extension of the product org and technical writing.

## Greg Baugues

What I think we can say objectively, with some humility, folks in the past used to say that Twilio had some of the best developer documentation around. What was it that was different about Twilio's docs versus what was more common for developer documentation back then?

## Andrew Baker

Yeah, I think it's a great question to dissect because part of what drew me to Twilio — and I'd already used the API as a developer hobbyist — Twilio had a reputation for great docs even before we started this team. That's because there was just such a "religious leap of faith" on the core hypothesis: you can build a company around an API as your product and a developer as your customer.

When the company was small and there wasn't a docs role, every engineer and product manager contributed to the docs and saw it as a critical part of that leap of faith underpinning the company. That gave us a head start. As the company grew, we got to create a team and really dive into documentation as a product mentality, which you hear people talk about a lot now, but back then there wasn't a lot of prior art. 

We had to start at first principles: for us as engineers, what were the best docs experiences we'd ever seen? Which open source tools or libraries inspired us? How could we figure out the right balance between helping a developer new to Twilio get to their first magical moment quickly, while showing them enough of the rest so they can finish building their use case?

That's really what the developer education team was responsible for: that moment between sign-up for your first API key, through the first five minutes with the product (hoping to get a magical moment), all the way to planning and launching a Twilio implementation, weeks or months later. Documentation was always the single most important pillar for supporting developers.

## Ricky Robinett

Andrew, I'm going to ask a leading question. One of the things I observed was a meaningful shift in the team's success with Kat's work around empathy-driven documentation. Can you lay that out? For many developers, empathy-driven docs opened our eyes to how to talk to people who don't get it innately.

## Andrew Baker

That's a really great point. Kat King's Talk is still online from Write the Docs—it’s an excellent piece of work I still link to. The mindset shift was crucial: in DevRel, people talk about org charts a lot. When you treat docs as a product extension and a cost center in R&D, it’s just a box to check on your way to releasing a product or feature.

The engineering work never gets done on time, and docs get compressed. If you staff with writers, they may do great prose, but can't always understand all the sample code, and how it connects. It's a black box process that becomes an afterthought, compressed when docs are part of R&D.

At Twilio, and elsewhere with great docs, we treated it as an essential component of business and the customer journey. Today you’d call it developer PLG (Product-Led Growth), but for us it was just self-service. Our job was to make the user (the developer) successful. We had to think about: what are the ways I can minimize the odds they go in a dead end? Or that they copy-paste code that won’t work, or that their account defaults don’t match an employee's?

That meant creating feedback loops. When Kat led the team, we shipped a five-star rating widget on every page: if you left less than five stars, you could leave a comment, and it went straight to a Slack channel the whole company could see. Not every visitor left feedback, but the trickle was enough to spot real problems. If you were logged in, we could sometimes reach out to help.

## Greg Baugues

Is there any way you can give us numbers to get an idea of scope? How many developers, how many products, or pages?

## Andrew Baker

I don’t have exact numbers anymore, but the unique thing was no user could become a customer without using the docs. Internally, we could say every customer needed the docs to work well.

The docs themselves added complexity as the company grew. Twilio was known for SMS and voice, but then added more products. What started as two icons grew to twenty, with varying depth and relevance. The challenge got bigger as we expanded.

I realized no user would use all the products. Our goal became: help developers get what they came for, without being overwhelmed by everything else.

## Greg Baugues

Ricky just pulled it: over 7,000 pages on twilio.com docs today.

## Ricky Robinett

According to Plush Cap, yeah.

## Greg Baugues

Amazing. We support maybe 10 products across 6–12 languages, most with helper libraries. There’s a ton to keep in sync, and for each one you’re working with product teams. What were some people/org challenges just keeping things up to date?

## Andrew Baker

We could spend an hour here. The most interesting part is how it changed. Early on, when starting the developer education team, there were only three of us, even though Twilio had 550 employees.

We knew we couldn’t write all the docs needed. The scope was too big for three people. So, we built tools so product and engineering could contribute. That worked while there was still a culture of contributing docs, but as we scaled, roles specialized. New hires didn’t expect to write docs themselves—many expected technical writers to do it.

That created a cultural challenge. Some product managers wanted to be hands-on, others wanted us to do everything. That made it hard to know what tools to build: should we optimize for everyone, or just for the docs team?

By the time I left, few product teams were hands-on at 5,000 employees. We were focusing more on being good stewards ourselves, with auto-gen docs and internal tooling for our pros.

## Greg Baugues

Go ahead, Ricky.

## Ricky Robinett

Yeah, Andrew, Greg, can I switch our topics a bit?

## Greg Baugues

Please, please.

## Ricky Robinett

People who know you well know you’re a great developer educator and a prolific builder. Can you talk about how, as a builder, your relationship with docs has changed regarding AI?

## Andrew Baker

It’s been mind-blowing. What we focused on was understanding customers and making every visitor successful. We created feedback loops: ratings, user testing, card-sorting exercises.

The past year and a half, I’ve been diving into AI tooling, curious what these tools are good for and what they change. Being a bootstrapper, I like seeing what one person can do. Now the challenge isn’t personally understanding a new API but how much I slow down, leave my IDE, and sign up for something. High-friction signup experiences frustrate me more than before. I just want my API key pasted in my editor so my coding agent can finish the job.

I think a lot about getting your docs into your IDE so your agent can access it. Stripe’s built-in doc fetcher is fascinating: you get up-to-date, vendor-approved info, even when ChatGPT doesn’t have your latest API changes.

## Ricky Robinett

So are docs no longer for humans, but for LLMs? Are humans using assistants to consume and learn docs?

## Andrew Baker

You could see that as a hot take. If I ran a team in 2025, I’d argue the most important audience is IDEs and agents, not developers themselves. But there’s an artistry to docs that help humans learn—ancillary skills, the first time you use an API, etc. That part is worth preserving.

For parsing through lots of pages to make one API call, though, the best workflow might be to give agents everything so they can apply it to the developer’s problem.

## Ricky Robinett

Let me tie that to something else. We spent a lot on robust templates and sample apps, but they didn’t have the impact we expected. Now I see more folks wanting templates that get them most of the way so their assistant can finish. Do you think templates will have a resurgence?

## Andrew Baker

Hot take: I disagree. More devs are comfortable starting from a blank IDE now. Maybe the best agents use prompts to find sample repos for inspiration, but I doubt people go to your docs just to clone a repo. The blank editor might be more important. Still, sample code on GitHub can help LLMs learn the right way to use your API.

## Greg Baugues

There’s a dichotomy: Developers consume docs via autocomplete (from old training data, maybe not from official docs), or via retrieval-augmented generation (RAG) using tools like Stripe’s MCP server. Even then, hallucinations are an issue. Any best practices to ensure the "proper" approach is in training data?

## Ricky Robinett

Quick Cloudflare answer: try everything. If you miss a training window, you might lose 12–18 months. Lots of samples, LLMs.txt and Markdown for LLMs. Haven’t seen RAG work well yet; it’s still manual. Also, docs links for crawling aren’t a silver bullet.

## Andrew Baker

It depends. There are two sides: if you’re an incumbent, stable API, LLMs know about you. If you’re a new startup, you have to find ways to get recent context into the dev’s environment.

I found Context 7 (from Upstash)—paste in a GitHub repo and it outputs a consolidated, LLM-friendly version (including LLMs.txt). I tried it and got a link for my dev environment. I’ll use it again.

## Greg Baugues

That’s great, and they even have an MCP server.

## Andrew Baker

I haven’t tried it, but yes.

## Greg Baugues

For a standard, stable library, autocomplete works well. For new tools and AI agents, LLMs might not know. The distinction between incumbents and startups is crucial—they have different problems.

## Ricky Robinett

In the old days, the best doc signal was being the top Google hit for "send SMS with PHP." Now you want to be the top query result in ChatGPT—with working, copy-pasteable code.

## Andrew Baker

Let me pitch my fever dream workflow. Feedback loops were huge for us—the best signal for making API/docs better. What if a dev integrated your MCP server in their IDE, and the agent could retrieve current docs and collect feedback on whether they solved the problem? This is realistic to experiment with.

## Ricky Robinett

Great idea, Baker. I’ve been trying automating tutorial testing with LLMs—not just code sample tests, but whole experience reviews. This is promising self-critiquing for docs/tuts.

## Andrew Baker

I agree; maintenance was the most painful part for us. If you could point an LLM at a URL, let it run and critique examples, I’d have paid for that daily on every page.

## Greg Baugues

Imagine running Twilio docs in 2015–16, but now with LLM API access. Where would you deploy these for maintenance?

## Andrew Baker

There are concerns in the technical writing community about LLM-authored docs. I’m more open to it. At Twilio, our philosophy was that sample code was most important—code is the densest information. That’s why we prioritized language support.

If you believe code is the most important, I’d use LLMs to get a first draft of the rest of the prose, grounded in truth. I wouldn’t let LLMs produce huge unsupervised outputs, but as a draft to support code? That’s valuable.

I’d also go further: point an LLM at the code itself, have it extract endpoints/params, generate sample code, and wrap docs around it. We generated API reference docs from the API's source of truth, which reduced maintenance and increased quality. Today, generating docs from OpenAPI is routine, but for us it was all internal tooling. Imagine letting LLMs generate public docs from real code.

## Greg Baugues

Suppose a startup just raised funding and needs to write docs. What product docs inspire you, and what are three top tips?

## Andrew Baker

Honestly, I haven’t seen new product docs that truly knock my socks off—it’s hard at a new company where resources are scarce and focus is on agents, not prose. If I started today I’d generate docs from the source of truth, keep code and doc context together, and leverage LLMs’ context windows on small codebases.

I’d implement an automated pipeline for OpenAPI docs, keeping context up-to-date, flat, and auto-exposed for LLM/developer consumption. Beyond that: MCP servers. They fill product lifecycle gaps—e.g., Neon’s runs queries live, Sentry’s investigates errors, custom ones let devs manage webhooks/dev tools. No one covers the whole lifecycle yet.

I wouldn’t build elaborate user consoles; I’d make signup quick: email, password, API key, and MCP link. Docs would be written more for agents than for direct humans.

## Greg Baugues

That feels like a hot take.

## Andrew Baker

You warmed me up, Ricky!

## Ricky Robinett

We’ve always valued dashboards visually, but they can become obstacles. I’d rather converse with my data, via MCP and integrations.

## Andrew Baker

Exactly. Even at Twilio, with great docs, we didn’t emphasize dashboards enough and it became a problem. Maintaining or using a weird UI isn’t fun—dashboards should be rethought.

## Greg Baugues

So the goal wasn’t "great docs," but "great dev experience." Docs were integral, but now agentic-first tooling might matter more—a single Markdown file, curl commands, etc. The best experience may involve not visiting your website at all.

## Andrew Baker

Right, I’ve wondered if you could just have an API endpoint that mints temp accounts/keys for dev IDEs—skipping the website altogether. Could agents register on the user’s behalf? That would be true frictionless onboarding and would let you skip building a marketing site.

## Greg Baugues

You almost want services to authenticate with a cursor account. Maybe a step too far, but interesting. Ricky?

## Ricky Robinett

I have many thoughts, but it's a wild topic. Andrew, what are you most excited about now, and how can people keep up with you?

## Andrew Baker

I’ll speak at DevRelcon in July on this topic, phases of PLG, and how things are changing. You can follow me on LinkedIn—look for Andrew Torque Baker. There are a lot of Andrew Bakers, but only one with the middle name Torque. This is an amazing time to work in DevRel, even after hard years. You get to expand your job description, org charts are flat, jobs are multidisciplinary—DevRel has always lived at that intersection. It’s a great opportunity to combine skills and inspire teams to try new angles.

## Greg Baugues

How do you see new folks writing first code, via new tools or as non-devs, changing DevRel, docs, and experience?

## Andrew Baker

That’s inspiring for me. We struggled to name that persona—maybe "builder" fits best. Someone building something from nothing, though they might not identify as an engineer. Twilio’s simplicity and magical results let us meet folks starting out in software, changing how they viewed work, careers, possibilities.

What’s interesting is the new motivations builders may bring. A few years ago, the wisdom was: find a tiny niche, keep it manageable, marketable. Big projects required VC, limited your options, dictated by investors. Now, maybe a tiny team can ship world-class software with little capital. If you once needed 100 people, maybe now you can do it with 3, 5, or 10. With the right group, different motivations (not just maximizing returns) could drive hard work and creative outcomes. That’s my fever dream for now: a new way for small groups to build what was out of reach before.

