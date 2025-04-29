# Level Setting 

what does a magical developer experience look like? 

examples: 
* twilio
* stripe
* openai 
* cursor
* assemblyAI 


# Developer Experience

- What does a magical developer experience look like with AI assistance? For example, could a developer signup for your product and get to hello world without leaving the IDE?

* Developers are leaving the IDE less than they used to. What tasks do developers currently accomplish by visiting your console that they could solve in the IDE via an agent? (eg, change a webhook? generate a new API key and save it to .env?)

- How do you help developers help LLMs to use your product? Prompts on your docs? .cursorrules and CLAUDE.md files in your repos? 

# MCP 

- What's unlocked if a developer installs your MCP server into their IDE? For instance, can you ensure they’re always using your up to date docs?
    
- Will MCP servers become the primary way a developer interfaces with your product?

# Training Data / Suggestions

- Few things frustrate a developer more than copy-pasting code that doesn't work. At Twilio we meticulously made sure all the code on the docs and blog worked. LLMs produce, almost by definition, "average code." How can you improve the odds that code suggested by LLMs for your product actually works the first time?
    
- LLMs are trained on outdated versions of your docs and SDKs. Their knowledge cutoff is 12+ months in the past. There will always be more outdated code in the training data than up-to-date examples. How do you think about backwards compatibility and versioning?
    


    
- We used to assume that if we had the best DX and the best docs, once a developer integrated with Twilio we would be super sticky. Customers would be willing to pay a premium on usage because developer hours was their scarcest resource, so vendor swapping would be too costly. How much vendor lock-in is there if a refactor is a cmd-k away?