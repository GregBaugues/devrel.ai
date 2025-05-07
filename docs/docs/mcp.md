# MCP and developer docs

MCP servers seems really useful if you are a API purveyor -- a vendor approved, first-party, up-to-date component in a developer's stack that's not just your SDK, but a tool that can help a developer across all phases and needs that a developer has when building with your product. 

Stripe's MCP server has tools built in to fetch the latest docs in to the IDE. It can access the most up to date information about how your API works in a way where Claude, Gemini, and ChatGPT might not know if your API has changed in like the past 6-12 months. 

After that, focus on MCP servers. The most interesting ones plug gaps across the workflow that aren't just about writing code: 

For example: 

* Neon (serverless Postgres) MCP server lets my agent run queries against production data for debugging
* Sentry's lets me investigate related errors

If you offer your own MCP server to let developers manage your product (e.g., webhooks) programmatically, that's powerful. No one's quite providing an MCP server that works across the whole lifecycle yet.

I wouldn't prioritize building elaborate user consoles. My signup would be quick: Email, password, API key, and instructions for plugging in the MCP server. If you want to look at the docs, you can—but I'd build docs more for developer tools/agents than for direct human consumption.