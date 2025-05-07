---
title: AI Native Docs
---

# AI-Native Docs

_Updated: 2025-05-07

This article is based off an [interview](andrew-baker-on-docs.md) with [Andrew Baker](../people/andrew-baker) and [Ricky Robinett](../people/ricky-robinett). 

---

In 2025, the most important audience for your docs is developers' IDE and their coding agents, not developers themselves.

The old way of building software was about: "how can I understand a new API or library that I'm incorporating into my product?"

Building with AI is about: "how much am I going to have to slow down and leave my IDE to incorporate a new vendor or API?"

Your goal is to help a developer finish building their thing as fast as possible. 

The best AI-native developer education workflow is one where:
1. you provide their agent with accurate information about building with your product
2. the agent applies your context to the developer's problem
3. the agent writes code that solves the developer's problem on the first try. 

How do you pull your docs into your coding IDE so that an agent can slurp up all the information that humans won't bother to read? 

----

There are primarily two ways that developers can consume your docs from their IDE/agent: 

1. Your code is included in the model's training data. 

2. Your docs are inserted into context at time of request, either by:  
	* The developer copy-pastes directly into context
	* The agent fetches the docs via URL
	* The IDE imports and embeds the docs and performs RAG 

# Getting in the training data


# Realtime Doc Retrieval 

 Stripe's MCP server has tools built in to fetch the latest docs in to the IDE. It can access the most up to date information about how your API works in a way where Claude, Gemini, and ChatGPT might not know if your API has changed in like the past 6-12 months. 

when using tools like Stripe MCP server. Even then, hallucinations are an issue. Do we have any idea about best practices to ensure the "proper" way of doing things is represented in the training data?

MCP servers seems really useful if you are a API purveyor -- a vendor approved, first-party, up-to-date component in a developer's stack that's not just your SDK, but a tool that can help a developer across all phases and needs that a developer has when building with your product. 

 Stripe's MCP server has tools built in to fetch the latest docs in to the IDE. It can access the most up to date information about how your API works in a way where Claude, Gemini, and ChatGPT might not know if your API has changed in like the past 6-12 months. 

---

# Writing AI Native Docs

Focus on generating your docs from the "source of truth" — keep code and doc context together, especially when you have a small codebase and can fit more in the context window that LLMs allow.

Implement a deterministic automated pipeline to generate OpenAPI docs. Keep everything up-to-date, flat, and automatically available so an LLM or developer can consume it without your supervision. 

Implement [[feedback mechanisms for your docs]]


----




