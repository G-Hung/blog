---
title: "How to choose jobs in the DS world"
toc: true
image: images/post/job_choice.png
comments: true
layout: post
hide: false
search_exclude: false
description: "My evaluation list on DS jobs"
categories: [career]
---

### How to choose jobs in the DS world?
 
This is what I have struggled in my mind over the years, what is a good DS job……. 
To solve this problem, I have created the checklist/questions which I hope the previous me could read before making the career decision. I won’t talk about compensation / tech details / interviews, that’s another story
 
You are not always in the position to choose (such as finding jobs during COVID-19) but you should seriously evaluate your options if you can
 
### Job nature
 
There are thousands of jobs sharing the same title, eg: data scientist, data engineer, ml engineer. But they could be totally different from company to company, be aware!
 
The first thing I will look into is the skill requirements to identify the job nature
 
If it is analytics, expect tons of SQL, dashboards, presentations, product analytics, experimental designs. You probably need to enjoy talking to people, finding insights, guiding the business, which means you need to be a domain expert in that business. In short, I think it is more like a business/PM/consultant type of roles, but from data perspective
 
If it is engineering, be alert if the job responsibilities are vague, don’t make assumptions, let me repeat: don’t make assumptions! For example, the people who share the data engineer title may do completely different things. Some are developing ETL pipelines; some are working on instrumentation; some are building the new data / ML infrastructure. You should think clearly whether that fits your career plan!
 
Also, another common “trap” is internal transfer, you want to get into the company first and switch to the roles you want, while I don’t deny the possibility, don’t be over-optimistic in your calculation, hope is not a strategy

If it is modelling, I will consider two things, one is the value of the models, another is the team maturity. For example, developing a model for Dogecoin price prediction sounds great but the outcome is probably not promising. Team maturity is  another consideration, be aware if the team is too green or even worse, you are the first member. They will sell like every startup does: you will have enough space to innovate. There are successful stories but think about survival bias. If you are super capable/team lead level, it may be worth trying; if not, then………
 
### Business/product model
 
Personally I think this is fundamental factor to determine your scope and potential achievements in the organisation, and financial uplift, I will ask myself the following questions:
 
1. How do you justify your (or your team) pay check in that business/product? How large is the potential uplift?
This question requires you to think about how the company makes for living, and what area you can contribute.
 
   For example, in the traditional industries such as merchandising, they probably don’t need advanced ML yet but they need to digitalise their business first. So even if you are a genius in ML, there are no such demands, and your deliverables will likely be ppt or fitting some models on some data in a Jupyter notebook. You will likely try to establish some KPIs or standardise the business workflow and get rejections from business experts.
 
   The trap here is these companies usually say they are willing to change/digitalise themselves, but that usually won’t happen because that doesn’t fit their previous success path, your role is in fact threatening the interests of the original core team if you can't show values quickly. Don’t recommend unless you are confident that you can be an asset rather than a liability.
 
2. What is the “resource complexity” to scale? O(1)? O(n)? O(n**k)?
Software industry is different from others because it is much easier to scale, or in economics terms, marginal cost of software approaches zero. But not every software has such a property, especially B2B solutions. In recent years, there are tons of “AI companies” developing their solutions in different verticals and plan to sell them.
 
   The happy flow is they will develop one algorithm/system and run in different customer systems, since the companies in the vertial are mostly giant companies [eg: banking, telecom, retailers, airlines], they can afford a big bill if the solution is nice! But the unideal parts are: selling solutions to business usually require custom integration, that hurts the scalability and increases the marginal cost, A LOT, especially if you are using AI [those deep learning things]. Deep learning models are still blackbox, there are too many edge cases if the business requires more than the simple & straightforward use cases.
 
   These companies can definitely make money if the margin is big but nature will become more like a service or integration company, aka human intensive. So from an employee perspective, it implies you will need to do one project after another, hence operational tasks / projects may take up significant amounts of your time and you have less time for R&D / innovative things if those are what you want.
 
   To compare the difference, imagine SaaS companies like Confluence [The company that makes Jira], the marginal cost to serve one more user is close to zero and even if they don’t develop any feature for a whole quarter, it won’t affect their growth in the short run. These companies hence usually have more time & resources to experiment the new things because the business outputs could be detached from employee’s work hours and client’s business logic
 
3. business/product model also affects the operations, A LOT!
We are doing DS so where is the data? SaaS / B2C products don’t feel such pains because users will likely use their developed applications, and engineers can implement tracking or log the events in servers to collect the data [there are also some headaches but everything is under your control, at least before Apple's App Tracking Transparency].
 
   But imagine if your clients are government, banks, airlines, retailers, and you have a ML solution for parts of their processes. Then you need to ask them for the data, you need to understand their schema & business logic, handling the dirty data, and come up with tons of workarounds to run your models.
 
   That isn’t fun because your time is tied to the outcomes & your work is constrained by others. Never imagine those companies will change their process because of your product, never assume their digitalisation level will boost suddenly to meet modern software requirements. You will probably be woken by PagerDuty and live with tech debts until the end of your tenure there instead
 
[Nice article](https://a16z.com/2020/02/16/the-new-business-of-ai-and-how-its-different-from-traditional-software/) from a16z to discuss AI companies
 
### Team
 
Your supervisor and team contribute a huge chunk of your job satisfaction, they can determine whether it is an amazing or nightmare experience. But this part is quite general for every job, some key signals I recommend you to look for are:
 
1. Growth mindset:
Do they adapt to a growth mindset? Do they encourage people to grow but not box them like a robot? Do they micromanage? How do they make the decisions? Are they humble? Get these information during interviews
 
2. Atmosphere:
Are they a happy team? Are they humour？Are they willing to share the insights and knowledges? This will signal whether people are psychologically safe, if the answer is no, you better understand why and whether you can accept that. Mental health and growth are even more important than your compensation after a certain threshold. A mismatched atmosphere will make you become a philosopher, stay away from the toxic culture, it makes you negative, short-term focus, and anxious!
 
3. Experience:
Are the team experienced? If not, you may have a hard time getting up to speed. BTW, companies usually frame this shortcoming as challenge / opportunity, calculate the odds yourself
 
### Company
 
1. Do due diligence carefully
Go to Glassdoor/Blind, check the negative reviews because they are mostly true. My theory is 5 star reviews could be neglected because that fits the company interest but you should read and evaluate every word in 1 star reviews
 
2. Check the background of management
Are they experienced? Do they know what they are doing? Do you have networks that work with/for them? Give them a call! These are important because inevitably there are up and down in business, these factors will take effect at that critical moment
 
3. Check company retention
Are there many people leaving recently? That maybe a signal
 
4. Check funding status if you are applying for a startup
 
5. Trust your guts
idk, but whenever I feel something weird / doesn’t make sense, they are usually true unfortunately. Be rational, don’t be over optimistic. Remember they are trying to sell you the company, which means they are like a sales team and show only beautiful pictures in your mind. Be rational!
 
### Conclusions
 
Unless you are super lucky and get your dream job, your decision should be tradeoff b/w various factors we discussed above
 
- Some people enjoy coding while some people enjoy talking to people
- Some people enjoy quiet culture while some people enjoy happy & open culture
- Some people prefer stability while some people prefer growth (risk)
- Some people prefer B2B because of easier monetization while some people prefer B2C because of possibility of rapid scaling
 
As long as you have evaluated the options carefully and understood the potential good and bad, the rest is your choice!

### Recommended reading:
[reading note of Effective Engineer](https://gist.github.com/rondy/af1dee1d28c02e9a225ae55da2674a6f)
