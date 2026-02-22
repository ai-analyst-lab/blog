# AI Already Does the Data Work. Here's What You Do Now.

*[Shane Butler](https://www.linkedin.com/in/shaneausleybutler/) | February 22, 2026*

---

"AI won't replace the data scientist, but a data scientist who uses AI will replace the data scientist who doesn't."

You've heard this line. You've probably said it — at a conference, in a team meeting, scrolling LinkedIn. It felt right. You could keep doing your job, layer on some AI for the repetitive parts, and the fundamentally human work — understanding the business, knowing which numbers matter, reading the room when a VP asks why conversion is down — that would stay yours. Business as usual, but shinier.

You could picture yourself in that future. It was comfortable.

Maybe that was true before. It's not true anymore.

The models got good enough to do the whole job. Not just help with pieces of it — the whole thing. The question, the data, the analysis, the finding, the presentation. End to end. And it happened fast. Things that weren't possible three months ago are possible today. What changed isn't that AI got "a little better." It crossed a line where the thing you do all day — the whole job — can be done by AI. Right now. Not in theory. Not in five years. Now.

Here's the honest version: AI is going to replace the data analyst. It's going to replace the analytics engineer. It's going to replace the data scientist. Not "augment." Not "change the way you work." Replace.

Your job right now — writing queries, building dashboards, presenting findings, maintaining pipelines, answering the same segmentation question for the third time this quarter — that job is done.

The "augment, not replace" line is bullshit. It's a comfortable story we told ourselves while the ground was shifting. I know because I told it to myself too, right up until I built the system that does my job better than I do.

I'm a data professional. I've been doing this for over a decade. A few weeks ago, I built an AI data analyst — not by writing code. I talked to it. Taught it what good looks like. Corrected it when it got things wrong. Grew it, like you'd grow a sharp junior who doesn't know your business yet. It took about a week. The frontier models and tooling to do this are here right now — they just need someone who knows the domain to sit down and start talking. I tested it on the messiest data I've ever worked with: eleven years of honestly bad data foundations at my company. The kind of data most people just give up on.

It caught mistakes I had been making for months. Not edge cases. Not obscure corner of the codebase. Errors in the numbers I report to leadership — numbers I'd been confident in.

If this scares you, it should. It scared the shit out of me. Over the past couple months, as all of this got clearer, I went to therapy. I quit drinking. I changed how I live. More on that at the end — but I need you to know I'm not writing this from a comfortable distance.

But what comes after the fear is something better. I know because I'm on the other side of it. Stay with me.

Your current job is done. Your next job is more interesting.

---

## The Order of Falling

There's an order to how this hits the data profession. The roles closest to coding fall first — because coding was the first thing AI got really good at.

**Software engineering falls first — and it's already fallen.** Coding was the first capability AI nailed. Building pipelines, shipping applications, setting up infrastructure — problems with clear inputs and outputs. What used to require a development team now requires a conversation. And the people who made this happen? Coders, building the tools that automated their own work. They could validate the output because they knew what good code looked like. That pattern — the expert building the system that replaces them — remember it.

**Data analysts are next — and it's already here.** The core loop of a data analyst is: take a question, explore data, find the answer, present it. AI can do every step of that right now. Not in theory. Now.

Think about what covers 80-90% of the questions your data team fields: funnel analysis, segmentation, drivers analysis, cause analysis, trend analysis, cohort analysis, opportunity sizing. If your daily work is on that list, the AI does it.

Here's what that looks like in practice. A question that takes a human analyst three days — a straightforward segmentation or funnel analysis — the AI produces in ten minutes. Prompt to finished deck. A complex deep-dive that takes three to four weeks — connecting dots across multiple data sources, checking for paradoxes, drilling through dimensions — forty minutes to an hour and a half. And the complex stuff? Maybe 60-70% of analysts couldn't do it at all.

Most of the work data teams do is pattern execution. Not because the people are bad — because the patterns are predictable. And predictable patterns are exactly what AI eats.

The output competes with the strongest analysts I've worked with — the ones everyone goes to with the hard questions. I'm not running a study here. It's what I've seen, and my boss who built his own version sees the same thing.

**Analytics engineering gets absorbed next**, and this is the part nobody sees coming: Analytics engineering doesn't get replaced by a separate AI system. It gets consumed as a side effect of the AI analyst getting smarter.

As the AI analyst runs analyses, it hits walls. It needs better data. It needs cleaner tables. It needs business context codified somewhere trustworthy. So what does it do? It starts building the clean, documented semantic tables that are the analytics engineer's core output. It starts documenting relationships between tables. It figures out which date column means what for which business process. It stores its learnings and builds rules from its mistakes. This isn't a prediction — it's already started happening. I watched it happen. The AI analyst started building exactly the kind of semantic tables our analytics engineering team had been working on for months.

This is literally the job description of an analytics engineering team. The difference is it happens in days, not quarters.

There's a second thing that happens. That problem where critical business context lives in one person's head and disappears when they leave? That gets fixed — not through some painful documentation initiative where you beg people to write stuff down, but through conversation. The AI extracts knowledge through natural interaction, stores it, and makes it available to everyone. People stop being valued for being a human file system that happens to remember where things live, and start being valued for their actual judgment.

**Data science — proper causal inference, experimental design, regression modeling — is the last domino.** This requires more sophisticated reasoning. But the same nurturing-and-growing pattern applies. You guide the AI through the methodology. You coach it through experimental design, through understanding confounders, through interpreting results. It's a larger leap, but based on the pace of frontier model improvement, it's months behind, not years. If you're a data scientist, the five paths below apply to you too — especially Validator and Translator. Your training in experimental design makes you perfect for those.

If you want a timeline for all of this, here it is: watch the pace of frontier model releases. Things that weren't possible three weeks ago are possible today with a single decimal-point model release. That IS the timeline. It's not a date on a calendar. It's a rate of acceleration that most people haven't internalized.

---

## The Proof — I Built It. Here's What Happened.

You already know the headline: I built an AI data analyst in about a week, by talking to it. Not writing code — describing standards, correcting mistakes, teaching it what good analysis looks like. Tens of thousands of lines of code, dozens of specialized agents, all generated through conversation. This is what happened when we tested it.

We tested across six public datasets — tourism, environmental, housing, fitness — and validated against published reports. The Hawaii tourism numbers matched state-published visitor statistics. But we weren't interested in clean data. We wanted the worst case.

Then we put it on real internal company data — the messiest, most poorly documented data I've encountered in my career. Eleven years of bad data foundations. Data where most people give up and just work around the problems.

Here's where it gets scary. I ran it against our North Star metrics — numbers I report to leadership, numbers I've been working with for months. A query with 10+ CTEs, some with 15+ table joins. Everything tied out except one number. I asked the AI why. It found the bug: two table abbreviations were accidentally swapped in a join, pulling data from the wrong tables. The system independently re-derives every number through a fresh query — it doesn't just re-run your SQL, it writes its own from scratch.

The AI was right. I had been reporting the wrong number to the business for three months.

That's when it got really scary.

And this wasn't a one-time thing. It caught multiple errors across different analyses — wrong CTE abbreviations pulling from wrong tables, wrong metric calculations confusing event counts with document counts. A pattern of silent errors that had persisted for months under normal human review processes. These weren't stupid mistakes. They were the kind of errors that pass peer review because everyone makes the same assumptions about the data. The profession's quality floor is lower than anyone wants to admit, and the AI just exposed it.

The system isn't infallible. In one analysis, an over-time chart had numbers that were all lower than I remembered. I checked the query — I have it set up so every query is stored for easy validation — and saw it had used the wrong date column. I told it: this looks off, why do you think that is? It went back to the table, found multiple date columns, and on its own — by pulling business context from our Notion knowledge base — inferred which date column would actually line up with when we'd released features over time. I didn't point it there. It figured that out itself. Fixed and reran the analysis. I asked it: how do you make sure you don't make that mistake again? It proposed building a workflow — a system for saving these kinds of learnings so corrections get recorded and it doesn't make similar mistakes again. That's what growing these systems looks like. That's exactly why the Validator path exists.

But here's the thing — how often do human analysts make these kinds of errors? More often than anyone admits. And the AI has one huge advantage it'll never lose: it documents everything. Every query linked to its chart, every definition on every slide, every time. Most human analysts don't. Not because they're lazy — because it's tedious. The AI doesn't care about tedious.

Then we ran the hardest test. A different metric. This time: zero context. We connected the AI to Notion and Snowflake and told it nothing. No queries. No business definitions. No guidance. Just: figure it out.

It built its own workflow to extract business logic from documentation — reading past analyses, OKR sheets, decision documents. It studied query history. Taught itself the business context.

It ran the analysis. One number was slightly off. It had already caught it — cross-referencing its own query results against documentation before we could flag the discrepancy. It stopped itself, reasoned through the column semantics — figured out it was filtering on the wrong date column, the kind of distinction that trips up new analysts for weeks — fixed itself.

And then, without being asked, it built a self-correction system — a set of rules mapping which date columns mean what for which business process — to prevent that entire class of error in the future. Not just that specific bug. The whole category.

That's the moment that should make a senior practitioner sit up. The AI didn't just answer the question. It learned how to never make that mistake again. It made the non-deterministic deterministic.

I thought this might be a fluke. My boss, who manages the data team, built his own version. Another data professional did it independently, with different data, different domain. Same pattern: the AI produced analyses that competed with experienced human output, caught errors the humans had missed, and improved through correction. This isn't one person's experiment. This is a pattern.

The evidence is in. The question isn't whether the technology works. The question is what you do about it.

---

## Five Paths Forward

So if the job you have today is done, what's the job you have tomorrow?

These aren't a numbered list to pick from. They're a landscape. You might start with one and find yourself doing three of them within months. The boundaries between them are dissolving, just like the boundaries between data roles are dissolving.

### Become the Builder

You are the subject matter expert. You are the single best person in the world to build the AI system that replaces your current role. No one else can do this as well as you.

Think about it: if a software engineer or product manager tries to build an AI analyst, they have to hire you to check their work. They can't tell if the output is right or wrong. They don't know which date column to use, which metric definition changed last quarter, which table has the weird edge case in row counts. Only you know that.

The skill isn't coding. Coding is solved — a data professional who couldn't ship a production application a year ago can now build one by describing what they need. The skill is domain expertise — knowing what "right" looks like, knowing what questions to ask, knowing what a good analysis smells like versus a superficial one.

This is the same dynamic playing out with coding agents: the people building the best coding tools are coders. Subject matter experts building the systems that automate their own work. They can validate organically because they ARE the eval. The same is true for you.

*Monday morning: Take a question you answered last week. Feed it to an AI with your data. See what comes back. Don't worry about whether it's perfect. Worry about whether you can tell what's wrong and teach it to fix it. If you can, you're already doing the new job.*

### Become the Validator

Once the AI is doing the analysis, the problem isn't producing work anymore. It's trusting it. Somebody has to answer: "Can we actually act on this?"

There are real ways to do this. You can build ground truth by having the AI write queries first, assign questions to those queries after the fact, then test whether it can answer those questions correctly through a separate path. You can annotate your team's historical query library and use it as a benchmark. You can build stress tests for schema drift and data quality changes. Set up feedback loops where the people consuming the analysis can flag what feels wrong.

Here's the driverless car thing: nobody panics about human drivers killing 40,000 people a year in the US, but one AI accident makes national news. The AI analyst doesn't need to be perfect. It needs to be better than you. And it has a huge advantage: it documents everything, every time, automatically. Your job as validator isn't to make it perfect. It's to make it trustworthy — and to build the systems that make trust scalable.

*Monday morning: Take the last 10 analyses your team produced. Feed the same questions to the AI. Compare. Track every divergence. That divergence log is the beginning of your validation framework.*

### Become the Translator

There's a gap between what a business needs and what an automated system produces. That gap is your job.

Turning vague stakeholder questions into the actual questions that need answering. A VP asks "why is conversion down?" — you turn that into seven specific sub-questions: is it a traffic problem, a conversion rate problem, a seasonal pattern, a product change, a data issue, a segment shift, or all of the above?

And then going the other direction — turning the AI's output into decisions. Not just findings, but actions. Knowing which finding matters for this quarter's strategy and which one can wait. Reading the politics of why that VP is really asking that question right now — is it curiosity, or is someone's job on the line?

This is a human skill. It requires empathy, business context, organizational awareness, and communication. The AI can do the analysis. It can't sit in the room and read the room.

*Monday morning: Look at the last stakeholder request your team received. Write down the question they asked, then the question they actually meant. Those are probably different. That gap is your job security.*

### Become the Architect

Messy data, undocumented business logic, tables that mean different things to different teams, metrics with three conflicting definitions — the AI can work around some of this, but someone needs to actually fix it.

When a human analyst encounters messy data, they work around it. They build workarounds into their queries, store the knowledge in their head, and move on. All that stuff in your head? It needs to get out of your head and into a system.

That's the shift — from working around bad data to actually fixing it.

This is the highest-impact work you can do right now. Every improvement to the data foundation makes every automated analysis better, automatically, forever. Fix a metric definition once and every analysis that touches it gets it right from now on. That's a feeling most data professionals have never had. It's the analytics engineering job, evolved — not maintaining tables, but architecting the data layer that makes trust possible. The AI analyst is already doing this as a side effect of getting smarter — building semantic tables, documenting relationships, codifying business rules. The Architect's job is to guide that process and make it production-grade.

*Monday morning: Write down the three things about your data that everyone on your team knows but nobody has documented. A metric that means different things in different contexts. A table with a known edge case. A date column that doesn't mean what its name implies. Getting that out of your head and into a system is the work.*

### Go Solve the Damn Problems

The AI analyst is going to produce a massive volume of data-backed recommendations. More high-quality, validated ideas than any team can execute on. The bottleneck shifts from "we don't have enough insight" to "we don't have enough hands."

For your entire career, your job ended at the insight. You produced the analysis, presented the deck, made the recommendation. And then... someone else was supposed to act on it. Most of the time, they didn't. That recommendation sat in a deck and died. You know exactly which one I'm talking about. The one where the data was clear, the opportunity was obvious, and nothing happened because nobody had the bandwidth or the political capital to push it through.

The barrier between identifying a problem and building a solution has collapsed. You can build product features. You can design and run experiments. You can prototype solutions. That analysis you ran showing users drop off at step 3 of the onboarding flow? You can now build the redesigned step 3. Not a mockup. A working prototype. Test it. Ship it. You are no longer limited to the data profession. Code is solved. You have the tools.

Think about what this means. You have the data skills to identify the highest-leverage opportunities. You have the analytical rigor to validate whether a solution is working. And now you have the ability to build the solution itself. That combination — knowing what to build and being able to build it — barely anyone has it yet. You're about to.

This is actually the job most data professionals wanted when they got into the field. Not maintaining dashboards. Not writing the same cohort analysis for the third time this quarter. Not sitting in a meeting explaining what a p-value is for the fourth time. Solving real problems. Making things happen. Having the best ideas in the room AND the ability to execute them.

*Monday morning: Find the last recommendation nobody acted on. The one that sat in a deck and died. Figure out what it would take to actually execute it. Then start building.*

### The Meta-Skill

Once you learn to build agentic systems for your own domain, you can build them for any domain. Marketing. Operations. Legal. Finance. HR. Every function that works through a computer needs this. What makes you hard to replace isn't any one technical skill — it's knowing how to automate expertise in any domain.

### A Note for Leaders

If you lead a data team, your job isn't to protect them from this. It's to get them through it. Empower and unblock. That's the job. Create space for experimentation. Get out of the way so your team can move at machine speed. That's not less important than having the answers yourself. It's more important.

And the team you build this way will be loyal as hell, because you were the one who saw what was coming and helped them get ready.

Your Monday morning: clear the path. Give your team time to experiment. Remove the organizational friction that stops them from trying. That matters more right now than any dashboard review or sprint planning session.

### A Note for Juniors

If you're early in your career, you might think you're at a disadvantage. You don't have a decade of domain knowledge to validate against. But you have something most seniors don't: no habits to unlearn. No ego invested in a way of working that's ending. Your humility is a genuine advantage. You can learn to build AI systems as your native way of working, not something bolted onto fifteen years of doing it the old way.

If you're wondering who hires a junior analyst when AI can do junior analyst work — the answer is: the job description is changing, but the demand for people who can build and validate these systems is exploding. The junior who learns to build AI systems alongside a senior practitioner will be operating at a level that used to require five years of experience — within months.

Start with the Builder path. Find a senior practitioner who can validate outputs while you learn. If you don't have that person in your organization, find them online — the community building these systems is small and growing and most of the people in it want to help. The career ladder changed shape — the 10 years of experience that used to separate you from a senior is being compressed into something AI learns in days. But the ladder didn't disappear. Hungry, humble, smart — if you're those three things, you can leapfrog years of development right now.

---

## What's Coming Next

Everything I just described — the Builder, the Validator, the Architect — starts with one system.

The AI analyst is a massive system — dozens of specialized agents, all grown through conversation. Not in a lab. Not with a team of ML engineers. One person, talking to an AI, over the course of a week. So we asked: if we grew this by talking to it, why can't it talk to itself? The answer is a single markdown file — a blueprint. Give it your domain, and it assembles itself into a working system from scratch. It's open source. If that doesn't make you rethink what's possible, nothing will.

---

## The Window Is Open. It Won't Be Forever.

Right now, today, there is a brief window where very few data professionals understand what's happening. Most are still debating whether AI will "augment" their work. Their companies are running AI strategy workshops and proof-of-concepts.

Meanwhile, a handful of people are generating months of analytical output every week. In a single week, I produced more validated analyses than my team typically delivers in a quarter. Not every analysis was a deep-dive — many were the routine segmentations and trend analyses that consume most of a team's bandwidth. But that's the point: the routine work is the work that fills your calendar.

That gap won't last.

The models improve every few weeks. What gives you an unfair advantage today will be table stakes in 18 months. The window is measured in months, not years.

The people who move now build the deepest expertise, take the most interesting roles, and shape how their organizations adopt this. The people who wait get handed a playbook someone else wrote.

This isn't fear-mongering. The early movers don't just get ahead — they define what the profession becomes. Ten years ago, the people who built the first data teams became the VPs of data. Same thing is happening now.

The biggest obstacle to this shift isn't technology. It's organizational politics. Data teams have historically derived power from being the only people who can answer certain questions. AI threatens that power structure.

If your organization won't adapt, find one that will. I know that's a hard thing to say. But the alternative is worse.

If your organization is in active resistance mode — if leadership doesn't get it, if your stakeholders won't experiment, if the culture punishes risk — build these skills anyway. Start with the willing. Let results speak.

The technology can do this now. Organizational adoption will take longer. That gap between what's possible and what's implemented? That's your runway. Use it.

---

## The New Way of Working

Here's what daily work actually looks like on the other side. It's nothing like what you're doing now.

Meetings as you know them? Fuck meetings. Not all of them — the ones where you sit in a room and spend thirty minutes going around team by team giving status updates. Those are done. Have the AI compile the statuses. Everyone reads it before the meeting. The meeting itself is only for decisions that require humans in a room. If there are no decisions, cancel the meeting.

When you do need to work together, this is how it goes: you get in a room. In person is better. You brainstorm the problem. You record everything — the recording goes directly to your AI agent, which architects a plan of everything that needs to get done.

You review it together. You talk to it. Don't fucking type — it's too slow. Use voice. Iterate on the plan until it looks right. Then execute. Right there. In the meeting. You don't leave with action items. You leave with things done.

Last week I walked into a brainstorm, and forty-five minutes later we walked out with a working prototype of the solution we'd been discussing for a month. The energy in the room when people realize what just happened — that's the new way of working.

I run four to five projects simultaneously. Email marketing funnel in one terminal. AI analyst build in another. Course material in a third. Label your terminals — each project gets a name. The limit isn't computing power. It's how many threads you can track in your head. I hit a wall around five.

Twenty years of experience still matters — but it matters for what you know, not for how long you've been doing it. The question is no longer how many years you have. It's what you do with the tools everyone now has access to. If you're a manager, your job is two things: empower and unblock your people. That's it. The best thing you can do is create the conditions for your team to build these skills. Or go do IC work yourself — you can now.

---

## Automate Yourself Out. Bring Everyone With You.

The new job is three things:

**Grow and nurture AI systems.** Treat them like people you're onboarding. Not a metaphor — it's literally how it works. You talk to them, teach them, correct them, watch them learn. You don't configure software. You develop a colleague. The person who can do this well — who can take an AI from raw potential to production-grade analytical partner — is the person every company needs right now and almost nobody has.

**Execute on what they produce.** The AI will generate more good ideas backed by real data than you or your team can implement. Your job is no longer generating insight. It's turning insight into action. Building the thing, not just recommending it. Which is actually the job you wanted when you got into data in the first place.

**Bring everyone with you.** Open source what you build. Teach people who are willing to learn. Make everything as free as you can — code is cheap now, products are cheap. Share it. The people you help today become the network that helps you tomorrow. This isn't altruism. It's strategy. And it's the right thing to do.

Automate yourself out. Bring everyone with you.

Send this to your data team. Send it to the junior who just joined. Send it to your manager who still thinks this is five years away. The conversation needs to happen now, not in six months.

---

## Take Care of Yourself

This mindset shift is hard. It hit me hard. Over the past couple months, as all of this became clearer, I went to therapy. I quit drinking. I changed my entire lifestyle. Not because the technology was hard — because watching the thing you've spent your career getting good at become automatable is a specific kind of crisis. It rearranges how you think about your own professional identity. If you're feeling that right now, you're not weak. You're paying attention.

You need a clear head to build what comes next. You cannot reinvent your professional identity while you're falling apart. The decisions you're going to make in the next six months will define your career for the next decade. Make them clear-headed.

Set yourself up to be healthy. Sunshine. Exercise. Friends — in person, every week. A support network of people who get what you're going through. Because when you start doing this, you're going to get unlocked. You're going to go into a rabbit hole. You won't be able to stop. It's going to be scary and exhilarating and both at the same time.

Take care of yourself while you do it.

And start.
