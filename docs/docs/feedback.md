# How to continuously improve your docs

Kat King led Twilio's Documentation efforts for a couple years. 

She gave a talk at Write the Docs conference back in the day.

![](https://www.youtube.com/watch?v=_HCmFvxxKaQ)

In Devrel people want to talk about the org chart a lot — even R&D people do too, everyone loves to talk about corporate org charts. When you treat documentation as an extension of the product and it's basically a cost center within your R&D organization, you sort of consider it a box you have to check on your way to releasing a product or a feature. The engineering work never gets done on time, and docs become an afterthought and the part of the work that's going to get compressed the most. 

If you staff it out with technical writers, they may do a great job on the information architecture and prose, but they aren't necessarily going to be able to understand all the sample code that's handed to them, or how it relates to all the other pieces of sample code in that documentation. So docs become a little bit of a black box process that's kind of an afterthought and gets compressed when you treat it as an R&D product extension. 

The way we did it at Twilio — and the way I think most companies who have excellent docs have treated it — is saying "this is part of our way of growing our business and our customer base. It's an essential component of our customer journey." 

These days people will use the term "Developer PLG" most often to describe this. Most of the time we just called it self service, if we called it anything. At Twilio for so long, we didn't really have any other way to sell our APIs, so it was just like air to us. We didn't describe this funnel any other way. 

But when you do it that way, like any marketing or sales or support team, you are thinking about: my job is to make this user, this developer, successful. I need to go and understand what problems they're hitting along the way with their journey and really take the time to think about what are the ways that I can minimize the odds that they're going to go off on a path that's a dead end. 

For example: 

* What are the ways I can minimize the odds that they copy and paste a piece of sample code that's never going to work just based on their development environment? 
* How does their new account have slightly different defaults than the accounts that employees use when they're writing the documentation? 

When you approach it with that philosophy, you realize you need to create feedback loops to understand how the docs are working and not working for customers. When Kat was leading the team was when we implemented the single best feedback loop we ever had back in the day: a five-star rating widget at the top and bottom of every page in the docs. 

A developer could drop in a five-star rating for that doc, and if it was anything less than five stars, we would ask them to leave a comment and assure them as best we could in the UI that it was not going to be a black hole that that comment went into. 

Instead, the rating and feedback went directly to a Slack channel that everyone on our team and inside the company could see. So when there was something wrong with the docs, you would get that steady little drip every day telling you whether there's a problem or not. Not every visitor to the docs is going to take the time to fill out the five-star widget — indeed, very few people took the time. But that ended up making for a pretty manageable drip of feedback in that Slack channel, where you actually could, as a human being reading it, pluck out the patterns and figure out what items we need to investigate further. 

We had it wired up so that if you were logged into your Twilio console at the time, we knew your account ID when you left that feedback. If we thought there was something specific going on for your account, we could actually look up your email address in our internal dashboard and reach out to you and say, hey, I saw you're having trouble with the docs. How can I help?


----

Let me pitch my fever dream workflow. I was thinking about how crucial feedback loops were for us—the best signal we had for making our docs and APIs better. If you could convince a developer to add your MCP server to their IDE as they integrate your API, the agent could retrieve the latest docs, and you could even add a feedback tool to collect anonymous feedback on whether the docs solved their problem. This sort of telemetry isn't a stretch and would be interesting to experiment with.

## Ricky Robinett

Great idea, Baker. I've been toying with removing the human from some testing. For example, using Claude code (or another tool) to consume a tutorial and run through it, critiquing it—not just testing code samples, but the whole experience. It's a step beyond what we did at Twilio, and while my tool isn't fully ready yet, the idea of self-critiquing docs and tutorials with LLMs is promising.

## Andrew Baker

I agree—it was one of the most painful aspects of maintenance for us. If you could point an LLM at a URL with access to code tools, and it could run and critique examples, that would have been huge for us. We'd have gladly paid to have that run on every page every day.