# Developer Relations in the Age of AI

# The old devrel playbook

Twilio was one of the first companies to focus on developer relations as the foundation of its go-to-market strategy. 

When I joined Twilio's Developer Evangelism team in 2014, our devrel playbook was built on: 

* *Magical developer experience*. Signup for an account and send your first SMS in five minutes. 
* *Great docs*. Copy-pastable code (that *works*) that supports devs on their journey from quickstart, to production, to scale. 
* *Technical blog content* to generate awareness and drive signups via organic and developer-social channels. 
* *"Be everywhere and be awesome."* IRL events. Speaking at, sponsoring, hosting hundreds of meetups, conferences, hackathons every year. 

AI is changing how developers write code, which will have a profound impact on how  devtool companies reach and serve developers. 

The devrel playbook from 2014 doesn't work anymore. 

Since I left Twilio in 2023, I've been building a bunch with AI, and advising AI companies on devrel. This site is an attempt to document what effective devrel might look like in the age of AI. I won't pretend to have all the answers, but I have lots of questions and a few smart friends. 

# Devrel in 2025 

## Developer Experience 

* What does a magical developer experience look like with AI assistance? For example, what would it look like if a developer could signup and get to hello world with your product without leaving their IDE? 

* We were meticulous about ensuring that the code on our docs and blog *worked*. Few things frustrate a developer more than copy-pasting code that doesn't work. LLMs produce, almost by definition, "average code." How can you improve the odds that code suggested by the LLMs for your product actually works the first time? 
  
* LLMs are trained on outdated versions of your docs and SDKs. The knowledge cutoff is typically 12+ months in the past. There's more outdated code in the training data than up-to-date examples. How do you think about backwards compatibility and versioning? 
  
* Developers leave the IDE less than they used to. What tasks do developers have to visit your console for today that they should be able to solve in the IDE? (eg, change a webhook? generate a new API key and save it to .env?)
  
* Will MCP servers become the primary interface between your product and developer tools?

* What's unlocked if a developer installs your MCP server into their IDE? How do you incentivize devs to do so? How do you make it really easy?  
  
* As a thought experiment, assume AI agents your customer instead of humans. What changes? 

* How much do you need to help developers understand how to prompt the models to use your product well? How much does this vary from model to model, version to version? 

## Docs 

* Should documentation be [primarily markdown-based](https://x.com/karpathy/status/1914488029873627597)? 

* There's two ways devs will interact with your docs from the IDE: the model's training data, and RAG over docs. How do you optimize for each?
  
* Is it a failure case to have a developer look at documentation at all?

## Technical Content / Blogs

At Twilio, we wrote different pieces of content to target Organic traffic vs. Social traffic. A post called "How to Send SMS with Python" performs well in Google, whereas "How I taught my dog to text selfies" performs well on Hacker News. The former drives signups, the latter drives awareness. 

I conceptualized this as "content a developer reads with an IDE open" and "content a developer reads on the toilet." 

* Re: "content a developer reads with an IDE open." Developers increasingly solve those problems with AI assistance, without leaving their IDE. Is there still value in shipping the "how to send sms in ruby" blog post? 
  
* For sake of argument: "search is dead, de-prioritize the blog," BUT you still need content to get included in the training data. The more content in the training data, the more likely the LLM is to suggest your tool. (Is this actually true, or does RLHF and fine-tuning counteract this?) 
  
* If that is true, are you incentivized to fill the internet with LLM generated technical slop to feed the training data? Feels like SEO in 2002. How do model providers curate training data to avoid this race to the bottom? 

* Are we all going to develop slop fatigue that makes a corporate blogs feel kind of gross, because we all know that that content is at least partially AI generated? 

* Do you now bifurcate your content strategy to "for humans to read" and "for AI to read?" 
  
* Whatever your strategy to get your code into the training data, the feedback loop is long. As of April 2025, o4-mini has a knowledge cutoff of June 2024 -- an 11 month lag. How will you know if your train-the-models strategy is working? 

* Will there be an Google AdWords equivalent for LLMs where (devtool) companies pay for preferential treatment? For a "small fee", will OpenAI let you be a "verified source" of training data, so that Twilio is recommended first when a developer asks how to send an sms in ruby? 

* Is your blog still the right place to publish code? Should you shift your content mix to be more open source repos on github? 

* Do humans still need copy-pastable code from your blog, or is high-level content more valuable: systems and architecture guidance rather than implementation details?

* Where are developers now discovering tools and APIs if not through traditional search?

* Does YouTube become a more important developer acquisition channel, since the bar for shipping content is higher, leading to less slop, and it offers connection with a real human? 
  
## Events

Perhaps less AI specific, but the devrel ground game changed a lot during the pandemic and post-ZIRP. 

* How are T&E and sponsorship budgets looking in 2025? 

* It seems like AI caused a resurgence of events, especially in SF. What are the most successful formats? 

* Are hackathons more or less powerful in the era of vibecoding? 
  
* Why get on a plane to speak to a breakout room of 60 devs or scan a few hundred badges in the booth when you can ship a YouTube video that gets watched by X0,000 viewers? How do you justify the benefits of IRL events that don't show up on a spreadsheet (and never have)? 

## Demographics 

"A developer is someone who solves problems with code." - Ricky Robinett

* A whole bunch of people who do not identify as a "developer" are now solving problems with code, thanks to vibe coding. Are you trying to reach, eg, the nurse that builds a schedule notification system for her floor? Should you? 
  
* [70% of Mr. Beast's viewers don't speak English](https://www.youtube.com/watch?v=wMW7-yk296U&t=2140s). English has been the dominant language for technical documentation. How does inexpensive translation impact the growth of global developer populations? Should every devtool product now be global by default? Why don't you have docs in Portuguese? 

* 22 year old junior devs are more likely to be AI-native. They consume content via YouTube and TikTok. 40 year old senior devs are more AI-skeptical and consume longform text based content.  
  
## Acknowledgments 

This is an ongoing project by Greg Baugues. The questions and thoughts here were cultivated through conversations with many friends, especially: Ricky Robinett, Andrew Baker, Matt Makai. 

If you have thoughts on any of these, drop me an email at greg@baugues.com. 