Ricky: 

Let me tie that to something else we've put effort into. We've spent a lot of time on robust templates and full sample applications, but it often felt like they didn't have the impact we expected. For the longest time, most people didn't seem to use them, though now I see developers wanting templates that get them most of the way there so their assistant can finish up. Do you think templates will have a resurgence?

Baker: 



Me: 

There's an interesting dichotomy: Developers can consume your docs via LLM autocomplete (from training data that's maybe a year old and possibly not heavily weighted for official docs), or via retrieval-augmented generation (RAG) when using tools like Stripe MCP server. Even then, hallucinations are an issue. Do we have any idea about best practices to ensure the "proper" way of doing things is represented in the training data?

Ricky: 

Quick Cloudflare answer, then back to Andrew. Our philosophy is to try everything—because if you miss one training window, you could lose 12–18 months. So lots of samples, LLMs.txt and Markdown for copying docs for LLM consumption. I haven't seen RAG work well yet; it's more manual than it should be. Dropping a docs link for automatic crawling hasn't been a silver bullet either.

Baker:

It depends, and maybe we're seeing two sides of the same coin. If you're an incumbent brand or API with stable, backward-compatible changes, you have less to worry about—LLMs know about you already. If you're a new startup, you have to find ways to get up-to-date context into the dev's environment.

I found a project called Context 7 run by the folks at Upstash. You can paste in a GitHub repo, it'll process all the docs in that repo and provide a consolidated, LLM-friendly version (including LLMs.txt), even if the project hasn't adopted the convention. I added a repo recently; it processed it and gave me the link I needed—an easy way to pull docs into the development environment. I'll use it again.

Me: 

As a developer, I feel a dichotomy: If I'm using a standard, stable library, autocomplete works great. But with new stuff—especially with AI agents—there's a gap when LLMs don't know how to use it. Your distinction between incumbents and startups is really crucial, because they have fundamentally different problems.

Ricky: 

In the early days, the best measure that our docs were working was that a Google search for "send SMS with PHP" returned our pages as the top results. Now, you want to ask ChatGPT and expect working, copy-pastable code. You want to be the first answer and have working code.
