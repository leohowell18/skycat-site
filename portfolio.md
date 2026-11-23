---
layout: base.njk
title: Portfolio - Leo Howell
---
# Portfolio - Leo Howell



Hi, I'm Leo. I build the systems that keep content accurate and useful at scale, and I make complex things simple for the people who use them. That means templates, quality checks, and AI-assisted tools that let my teammates do expert work without needing to be experts in the systems underneath. Before that, I spent years as a writer and editor at ESPN and MLB. I'm also a cat dad with a 91% success rate on New York Times' Connections, and a fun addition to any meeting. Check out some of my work below, and feel free to add me on [LinkedIn](https://www.linkedin.com/in/leo-howell/)!



---



## What I've Built



### 🧪 AI-Assisted QA Tool with Claude Code



**What I did**



Spotted an unowned bottleneck and built a testing tool with Claude Code that fires any message scenario on demand, so our team can test our real-time content product without waiting for live games (or digging through historical events that might not even match the scenario we need).



**How I did it**



- Used Claude Code to build a tool that constructs mock data matching our system's expected data structure.

- Wired it into the same logic triggers production uses, so generated values stay realistic and in range instead of random placeholders.

- Designed it for editorial teammates without a technical background, not just engineers.

- Handed the prototype to engineering, who integrated it into the production QA stream, then trained the team and drove follow-on improvements.



**Why it mattered**



- Cut testing on a new push product from days or weeks to hours. No more waiting on the sports calendar to validate a fix.

- About half the content team now uses it near-daily, removing a bottleneck that used to sit entirely on me.

- Lets the team catch and fix issues before launch instead of during live events, when the stakes (and the audience) are highest.



### 🛡️ Catching the Errors People Can't See



**What I did**



Built layered quality checks for a live messaging pipeline handling millions of events on a typical game day. The checks catch errors human review misses, like a stat that looks believable but is the wrong one.



**How I did it**



- Defined what "broken" means for our content, including a two-tier error taxonomy: showstoppers, and issues that are acceptable but should be fixed. That pulled the serious problems out of general alerts and feedback, and cut the noise from minor ones.

- Wrote more than 20 SQL monitors that catch bad data, rendering problems, and logic flaws, and validated each one against real output before turning it on.

- Chose SQL over AI review on purpose: no added cost, no outside dependencies, and something one person could ship.

- Built a self-serve app that takes colleagues from a flagged message straight to the template editor to fix it, no SQL access needed.



**Why it mattered**



- A whole class of errors now gets caught before customers see it.

- Fixing problems became self-serve instead of a request to me.



### 💎 Turning Editorial Standards into AI Review



**What I did**



Set up two Gemini Gems that let my colleagues review content with AI, no technical help needed. One checks CSVs of content output against instructions and context I wrote. The other reviews Jinja2 template code against how our system actually works.



**How I did it**



- Wrote the instructions and context each Gem works from: our standards, the mistakes we see most, and how our templates and data fit together.

- Designed them for teammates without a technical background, so anyone can paste in content or code and get a useful review.

- Shared them through the team's Google accounts so they're part of everyday work, not a tool only I run.



**Why it mattered**



- Turned standards that lived in my head into a review tool anyone on the team can use.

- Gave writers a fast first check before content reaches me or goes live.



### 🧩 Making Personalization Safe



**What I did**



Built a Python helper library and shaped the data layer of a templating system that lets a small team of writers produce thousands of personalized messages across hundreds of scenarios, without writing conditional logic.



**How I did it**



- Shaped role-based context (subject and opposing team, offense and defense, leading and trailing) so writers can say who without working it out themselves.

- Wrote helpers for recurring editorial problems, like a vs. an, AP-style numbers, possessives, and stat formats.

- Made every helper fail gracefully: when data is missing, it returns nothing instead of breaking, so a bad feed produces a shorter message, not a broken one.



**Why it mattered**



- Writers focus on the message, not the logic.

- Personalization at scale stays readable even when the data isn't perfect.



### ⚙️ Live Messaging Product from 0 to 1



**What I did**



Drove the content side of a brand-new real-time push notification product for our customers: the content operations, QA processes, and templates that turn live data into accurate messages. I served as the bridge between technical and business teams, turning customer requirements into something we could build, test, and ship.



**How I did it**



- Got my hands dirty with SQL, Jinja2, Git, and AI tools to remove bottlenecks and take on more of the work the launch needed.

- Used years of sports media experience to craft message logic that mattered to customers while heading off problems and errors before they happened.

- Worked closely with data engineers and product leaders to shape quality checks and improve messaging based on customer feedback and performance data.



**Why it mattered**



- The product has grown into a seven-figure enterprise upsell.

- It now delivers live messages to millions of users.



---



## What I've Done



### 🛠️ Salvaging a Six-Figure Partnership



**What I did**



Stepped in to save a failing business relationship with a major professional sports league where content was not meeting customer needs and standards.



**How I did it**



- Bridged the gap between technical capabilities and the league's requirements to ensure data was ingested, available, and properly displayed.

- Overhauled content templates using subject matter expertise, data structure familiarity, and content strategy experience to rebuild client trust and produce high-quality outputs.



**Why it mattered**



- Regained customer trust through direct communication and demonstrated value.

- Turned around the relationship from on the rocks to earning a renewal.

- Demonstrated my customer empathy and ability to deliver under pressure.



### 🧠 Challenged Legacy Language at ESPN



**What I did**



At ESPN, I initiated a shift away from the term "owner" in fantasy sports, noting its racial and historical baggage and pushing for a change to "manager." I got the attention of the right people, aligned content and product stakeholders, and led updates across editorial and product to change the wording within a week of our first meeting on the topic.



**Why it mattered**



This wasn't just about language. It was about aligning our product and content with modern, inclusive values, something users had started noticing and questioning after missteps by other media outlets (and ESPN's television producers). The change is still in place today, and it reflects how I operate: by surfacing hard conversations and ensuring my team's work stays ahead of the curve and delivers content that respects its audience.



### 💻 Learning to Code to Remove Bottlenecks



**What I did**



Proactively taught myself SQL, Jinja2, and Git workflows to eliminate bottlenecks between engineering and business teams at Data Skrive. Went from relaying questions back and forth to directly building data models, writing template code, and having technical conversations about feasibility.



**How I did it**



- Learned SQL and relational database concepts to translate raw data into content objects that non-technical writers could use.

- Taught myself Jinja2 when the company pivoted to code-based content systems, becoming the bridge that enabled editorial teams to contribute without engineering dependencies.

- Integrated AI tools and Git workflows to automate repetitive tasks and speed up iteration.



**Why it mattered**



- Eliminated technical dependencies: could answer customer questions and build content templates without waiting for engineering availability.

- Reduced vertical launch timelines by 90% by handling data modeling and template creation directly.

- Enabled the company's pivot from CMS-based to code-based content systems by bridging the technical and editorial teams.



---



## Things I've Written



### ⚾ [Fantasy Baseball 101](https://www.espn.com/fantasy/story/_/id/22335040/fantasy-baseball-espn-fantasy-baseball-101-help-how-play-fantasy-baseball) - User Onboarding Content System



Created Fantasy Baseball 101 to remove signup friction and improve user satisfaction. A full beginner's guide built for clarity, onboarding, and search.



**Why it matters:** A plain-English guide to a complex game, built to help beginners sign up, get started, and stick around. Built for clarity first, with search in mind.



### 📈 [What Do We Mean by Scalability?](https://dataskrive.com/what-do-we-mean-by-scalability/)



A breakdown of why sports content is so hard to produce at scale (the calendar never stops, and every event already has competition for the SERP) and how automation lets brands show up for events, teams, and searches they'd otherwise miss.



**Why it matters:** Translates a technical, data-driven product into a clear business case for a non-technical B2B audience. Shows the same "why it matters" thinking that shapes my internal strategy work.



### 📍 [Create, Deliver, and Scale Hyperlocal Sports Content That's Valuable to Your Fans](https://dataskrive.com/create-deliver-and-scale-hyperlocal-sports-content-thats-valuable-to-your-fans/)



A look at how hyper-local, team-first content outperforms bigger national coverage for engaged fans, and how something as small as word order in a headline can shift how content ranks and resonates.



**Why it matters:** Combines SEO strategy with an understanding of audience psychology, and makes both accessible to readers who aren't SEO experts.



*Other bylines from past roles [can be found here](https://www.clippings.me/lhowell).



