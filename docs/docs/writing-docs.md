# How to use AI to help write developer documentation

Our philosophy at Twilio was that the sample code on the page was the most important part, because code is the densest way to convey information — assuming it's in the right language for the user. That's why we prioritized language support so heavily. 

If you believe that the sample code is the most important part — and arguably even more so now — I would look for ways to get a first draft of the rest of the prose that's as grounded as possible in the truth. 

Of course, you wouldn't want LLMs to generate thousands of words without supervision, but having them draft is valuable, since prose is one of the most time-consuming aspects.

I also wonder if you could go further: Point an LLM at the source of truth code, have it extract the endpoints and parameters, generate sample code, and then wrap a doc around it. 

The best thing we did at Twilio was to generate our API reference docs from the source of truth behind Twilio's APIs (before OpenAPI compliance was even a thing). That reduced our maintenance burden and increased quality. 

Today, generating API reference docs is routine if your API is compliant, but for us it was all internal tooling — we generated docs from the API's source of truth. It makes me wonder how much further you can go, having LLMs generate the public docs based on the real code.