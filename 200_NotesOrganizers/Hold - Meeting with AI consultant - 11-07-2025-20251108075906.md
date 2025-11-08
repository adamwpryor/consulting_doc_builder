# Hold - Meeting with AI consultant - 11/07/2025

**Attendees:** Melissa Ghera, Ph.D., Adam Pryor, Bethzaida Sosa (SJF), jwelch
[https://t9014294891.p.clickup-attachments.com/t9014294891/c06d7848-764e-449a-b396-7939e03ecaa1/c06d7848-764e-449a-b396-7939e03ecaa1.mp4?view=open&filename=Hold%20-%20Meeting%20with%20AI%20consultant%20-%2011-07-2025.mp4](https://t9014294891.p.clickup-attachments.com/t9014294891/c06d7848-764e-449a-b396-7939e03ecaa1/c06d7848-764e-449a-b396-7939e03ecaa1.mp4?view=open&filename=Hold%20-%20Meeting%20with%20AI%20consultant%20-%2011-07-2025.mp4)

## Overview

The meeting focused on exploring an AI-driven solution to modernize the outdated catalog and curriculum proposal processes. The group discussed integrating disparate systems such as Banner, WordPress, and Brightspace to reduce manual errors and streamline scheduling and course conflict resolutions.

## Key Takeaways

* The team agreed to simplify the project proposal by concentrating on automating descriptive analytics and fact-checking course changes.
* There was a consensus on the necessity to overhaul manual ETL workflows and improve the integration between existing systems.
* Participants emphasized the importance of standardizing departmental data, including SQL queries, course maps, and templates, to support a smoother transition.
* A follow-up session with key stakeholders, including discussions with Kevin, Amy, and cabinet members, was proposed to review process maps and align on integration strategies.

## Next Steps

* [ ] **Adam Pryor**: Revise and streamline the project proposal to incorporate key AI integration recommendations and share it with the team.
* [ ] **Jason Welch**: Provide detailed SQL queries and documentation of the current ETL process for further review.
* [ ] **Bethzaida Sosa**: Distribute contact information for all key stakeholders and schedule a follow-up session with Kevin, Amy, and cabinet members to review process maps.
* [ ] **Melissa Ghera, Ph.D.**: Share documentation or details of the scheduling work already completed with Adam Pryor for review and integration into the project planning.
* [ ] **Adam Pryor**: Consult with a change management expert to address potential faculty resistance during the system transition.

## Key Topics

* **Review of Provided Files & Prototyping Discussion** Update
  * Adam mentioned he had begun prototyping using the files provided by Bethzaida and observed that it was feasible with the current data structure.
  * It was noted that the prototype worked well, emphasizing the need for integrating directly with the SIS for data output.

* **Catalog Differential Analysis vs. Change Tracking Bot** Update
  * Bethzaida explained feedback on the initial proposal regarding the change log generator and whether it should be a catalog differential analysis or a specific change tracking bot.
  * The discussion focused on the bot's role to track additions, modifications, and subtractions across multiple programs, ensuring appropriate follow-up actions.
  * Jason provided further clarification on how the output is expected to compare new proposals against the existing catalog.

* **Details of the Existing Catalog Process and Legacy Systems** Problem
  * Jason Welch elaborated on the two separate process flows: one for courses and another for curriculum proposals, noting that they are reconciled manually.
  * He outlined that course changes follow an electronic form workflow that eventually makes its way from Banner to WordPress via customized ETL processes.
  * There were concerns over the brittle and labor-intensive ETL process, partly due to the dated integration between legacy systems (Banner, WordPress, Brightspace).

* **Faculty Scheduling and Curriculum Conflicts** Problem
  * Melissa provided insight into challenges with faculty scheduling preferences and the resulting conflicts in course timing, for example between Organic Chemistry 2 and Calculus.
  * She explained that while some courses have rigid assigned time blocks, disruptions and inconsistencies arise due to differing faculty preferences, jeopardizing student progression.
  * The need to cross-check course rotations and four-year plans was highlighted as crucial to avoid scheduling conflicts.

* **AI Integration and Automation Potential** Idea
  * Adam proposed the development of an AI bot that could automate fact-checking of curricular proposals against the current catalog, validate course changes, and simulate student enrollment to detect conflicts.
  * The group discussed that the AI tool could transform current manual processes into a more efficient, descriptive analytics system that reduces human errors in scheduling and catalog updates.
  * There was also mention of using AI to reformat and standardize catalog templates to form a more cohesive handbook-like output.

* **Data Infrastructure and Process Standardization** Problem
  * Participants noted the importance of obtaining solid, standardized data such as four-year program maps, course rotation schedules, and departmental templates.
  * There was a consensus that much of the essential information exists only as unwritten knowledge among department chairs, hindering effective automation.
  * The need for a unified data repository or data lake as a foundational element in future solutions was raised.

* **Systems Integration and Technology Considerations** Problem
  * The discussion stressed the challenges presented by disconnected legacy systems, with an emphasis on the lack of seamless integration between Banner, WordPress, and Brightspace.
  * Adam and Jason debated the feasibility of using AI wrappers over existing systems, noting that without customized integrations the solution would be brittle and prone to failure.
  * The idea of potentially involving external vendors, like the mentioned example of Dewey, was brought up but concerns about high costs and long implementation timelines were noted.

* **Change Management and Faculty Resistance** Problem
  * A critical concern was raised regarding potential faculty resistance to an AI-driven system that might curb their scheduling autonomy.
  * It was acknowledged that while 80% of faculty might adapt to the changes, a minority could object strongly, necessitating robust change management strategies.
  * Adam highlighted the importance of demonstrable test cases to secure campus-wide buy-in and reduce resistance over time.

* **Refining Project Proposal & Next Steps** Decision
  * Adam stated he would amend and streamline the project proposal to focus on addressing the most pressing pain points, particularly automating descriptive analytics.
  * Jason was asked to share details of the SQL queries and ETL process to help diagnose integration issues.
  * Bethzaida committed to forwarding key contacts and organizing follow-up sessions, including an in-depth process mapping session with stakeholders such as Kevin and Amy.
  * The overall timeline mentioned was aiming for fall 2027 as a target start date for full implementation, which would align with budgeting and phased RFP processes.

* Transcript

    **Bethzaida Sosa (SJF):** Good morning.

    **Adam Pryor:** How are you?

    **Bethzaida Sosa (SJF):** Good. It's very early for you out there, isn't it? No,

    **Adam Pryor:** it's not too bad.

    **Bethzaida Sosa (SJF):** Okay. I

    **Adam Pryor:** was about to say I've. I've gotten the children off to school, so everything's fine.

    **Bethzaida Sosa (SJF):** Okay. That's the first check mark, right. Of the day. That's

    **Adam Pryor:** right.

    **Bethzaida Sosa (SJF):** Everything

    **Adam Pryor:** else can go fine from there on out.

    **Bethzaida Sosa (SJF):** Yeah.

    **Adam Pryor:** I. I sent you kind of a long email. I know.

    **Bethzaida Sosa (SJF):** And I haven't. I feel bad because I haven't gotten through it. I have time

    **Adam Pryor:** to

    **Bethzaida Sosa (SJF):** sort through it.

    **Adam Pryor:** The. The gist of it is I. I started playing with the files you sent.

    **Bethzaida Sosa (SJF):** Yeah.

    **Adam Pryor:** And this is it. I. I'm glad we'll have this kind of time to check in, because I. I could certainly build a prototype out of that. There's no, like. There's no question, like, we could do a little bit of that. And it went. It actually went pretty well, the prototyping. There's just. You. You really want to build this out of the SIS as directly as possible.

    **Bethzaida Sosa (SJF):** Okay.

    **Adam Pryor:** There are law. And

    **Bethzaida Sosa (SJF):** not from a fight, not from files produced yet from the raw data. Yeah. Okay, Got it.

    **Adam Pryor:** Yeah. Mostly because I'm. There's got to be a ton. I just can't figure out where some of this narrative text is coming from.

    **Bethzaida Sosa (SJF):** Okay.

    **Adam Pryor:** Like,

    **Bethzaida Sosa (SJF):** some

    **Adam Pryor:** of it I can. Some of it I can tell really, really easily. Like, when I look at the xml, I'm like, oh, okay. Like, here's. Here's. They've run a. There's some sort of ETL going on. Right. Like this out of probably some sort of cognos. It's

    **Bethzaida Sosa (SJF):** a homegrown system that. Ye.

    **Adam Pryor:** Right.

    **Bethzaida Sosa (SJF):** And ages ago. So it's not.

    **Adam Pryor:** Yeah. And I can. I can see. I'm like. Okay, so, like, these steps make sense to me. Like, you're pulling the report. You're running the report against it. It's probably a pretty clean data file. No problems asked. And then there are, like, these sections that I'm like, there's. I can't imagine how this is going other than handwriting.

    **Bethzaida Sosa (SJF):** Okay.

    **Adam Pryor:** And that's. That's kind of what I want to figure out, because I think that will help us.

    **Bethzaida Sosa (SJF):** Okay. Figure

    **Adam Pryor:** out how to move forward.

    **Bethzaida Sosa (SJF):** All right. Hi, Jason. And Melissa's joining. Hi, Jason. Melissa. Thank you

    **jwelch:** for

    **Bethzaida Sosa (SJF):** joining. So, Adam, for introductions. I think you met Jason Welch earlier this week. So Jason Welch is the registrar and Melissa is associate Pros. I forget. Assistant versus associate. Okay. Associate and provost. Associate Dean. Not

    **Adam Pryor:** provost. Oh,

    **Bethzaida Sosa (SJF):** my goodness. Yeah. Associate. I. Yes. Associate dean for arts. And sciences. So that is our largest school and that's why we've been having more dedicated conversations. And Melissa and Jason were provided direct input into those process flows and are directly involved in many of those processes. So Melissa, Jason and I did meet yesterday for a while actually, and yesterday was Melissa's first time reviewing the proposal. And really I just gave her a bird's eye view and we

    **Adam Pryor:** talked

    **Bethzaida Sosa (SJF):** a little bit about some specific bot recommendations and we have some feedback that I think is very helpful because they are ultimately the doers and see this process executed firsthand. So before we get too far in, I thought that we would discuss their feedback and go from there.

    **Adam Pryor:** Just FYI, I've got my note taker on, which is mostly about later on. I like to make sure that I didn't miss something while I'm writing things down. If you want me to turn it off, I will. I don't have any problem with that. But I wanted to tell you before I leave it on there,

    **Bethzaida Sosa (SJF):** I'm okay with it. Okay,

    **Adam Pryor:** we're going to just roll with it then. Great.

    **Bethzaida Sosa (SJF):** Okay, so these are the notes. So the process which we took during the meeting is I pulled up the proposal and we went through line by line with of the. The intervention AI bots. So the first thought was that the first one, the number one, the catalog differential analysis or the chant, the change log generator as it was written, the perspective was that it wasn't going to be as helpful, that a change log wasn't going to be as helpful, but change tracking for a specific purpose would be beneficial. So the thought was that a bot that tracks, that identifies additions, modifications, subtractions for course or programs that span across multiple programs would be beneficial and it will help expedite it because sometimes they're not always identified and the proper actions can be taken when it is a change spans across multiple programs. Okay, so that was the thought there. And I don't know how that differs from what you initially considered in the change log generator.

    **Adam Pryor:** I guess not significantly. I think the big thing is help me understand a little bit what you want the output to look like. I'm

    **Bethzaida Sosa (SJF):** going to defer to Jason.

    **jwelch:** The output to look like. So presumably in this scenario we get a curricular proposal from somebody. Let's just say it's Melissa, okay? Because she sent me the most recent one and it goes into this bot thing and it, the bot thing then reviews the proposal against the catalog and then it generates something that says here are the programs affected and this is how. Okay,

    **Adam Pryor:** so beside

    **Bethzaida Sosa (SJF):** that's

    **Adam Pryor:** okay. That's what I thought you were asking for. And this is sort of one of the things we specifically removed. Right. This. This is work that you would do at the level of proposing new changes. Right. It wouldn't be in the catalog. Like, this wouldn't be about the catalog per se.

    **Bethzaida Sosa (SJF):** Oh, the curriculum proposal. Right.

    **Adam Pryor:** This is a curriculum piece which is

    **Bethzaida Sosa (SJF):** what

    **Adam Pryor:** we had extracted from the original proposal in its entirety. Yeah.

    **jwelch:** But when we do curricular proposals, we start with the current catalog requirements.

    **Adam Pryor:** Totally agree. I'm on board. That's why I had put it in. In the original proposal. My suggestion is you all on campus are going to need to. To huddle up and figure out what you need, because I'm now getting sort of pushed in. Exact.

    **Bethzaida Sosa (SJF):** Yeah. Because Kevin said no to any. Not. Not to start

    **Adam Pryor:** with the curriculum.

    **Bethzaida Sosa (SJF):** Yeah. Well,

    **jwelch:** if Kevin said no, that's. That's one thing. But beside

    **Bethzaida Sosa (SJF):** me

    **jwelch:** for.

    **Bethzaida Sosa (SJF):** I did. I did well. And that's where, as we've seen. Right. There's what actually happens, and then there's the thought and understanding of what people think happens. And I think Kevin's pushback on not starting with the curriculum proposal. He was thinking more so on the approval side, because the approvals take 18 months and we won't be able to effectively make changes on time. Right. So. But this is a recommendation and an ask, so I think we should keep it. So should I change it different? That is not catalog change. That's

    **Adam Pryor:** okay. If you notice, after this, I will be able to sort of square this way. So, Jason, let me just get this straight. Like, just brass tacks. You need a document that when someone brings you a proposal for something that's going to happen in the new catalog, it's going to quickly roll through the current catalog and look for any place where that affects a different program. Yeah. Okay. We're going to kind of one line, some of the goals here just to. Yeah.

    **Bethzaida Sosa (SJF):** Smooth

    **Adam Pryor:** it out. Okay.

    **jwelch:** Anything you would add to that from your end, Melissa?

    **Adam Pryor:** Got it. Okay.

    **Bethzaida Sosa (SJF):** All right. And then we there. We skipped through, you know, 2,

    **Adam Pryor:** 3,

    **Bethzaida Sosa (SJF):** 4, 5, and 6 there. Didn't see the benefit of that one. There was thought that takes more time. It's. It's really about the human tasks. Okay. Completing it rather than the efficiency of it. Okay.

    **Adam Pryor:** I'm gonna. I'm gonna take off my consultant hat for a minute and put on. Yes,

    **Bethzaida Sosa (SJF):** please do my

    **Adam Pryor:** old

    **Bethzaida Sosa (SJF):** provost

    **Adam Pryor:** hat. Yes.

    **Bethzaida Sosa (SJF):** Okay. Tell

    **Adam Pryor:** me how faculty. Tell me how the scheduling process works. I don't. I don't care what's written on paper. Right now what I care about is how do you all actually get this done? And I'm going to give you a classic example for me, right? I had a department where no one wanted to teach other than 10 to 2 on Tuesdays and Thursdays. Yeah, that was unacceptable. So they submitted their preference and I ignored it. Right. That was the culture at my institution that I could get away with to say that was nice of you to say that that's what you wanted. That's not how this works. You are on contract. You are to be here. And I had people quit over it and we were okay with that. I am getting the sense that is not the kind of culture that exists at sjf.

    **Melissa Ghera, Ph.D.:** Kind of. And no, all at the same time. I mean,

    **Adam Pryor:** our

    **Melissa Ghera, Ph.D.:** biggest time block Crunches are still 9:30 to 3, Tuesday,

    **Adam Pryor:** Thursday

    **Melissa Ghera, Ph.D.:** shifts. What time block in there? You know, which two out of those four time blocks are most heavily populated depending on the semester. Right.

    **Adam Pryor:** We

    **Melissa Ghera, Ph.D.:** have worked, however, over the last five years to spread out the schedule more. Okay. So that we are less pro. We are in a less problematic state now than we were. So I think where I got hung up on what was written when we met yesterday, not having been in conversations again from since May until now.

    **Adam Pryor:** Yeah, it's

    **Melissa Ghera, Ph.D.:** like, what are we talking about when we're talking about faculty preference? If we're talking about give me your time block, I'm like, I don't really care what you. What your preference is

    **Adam Pryor:** for

    **Melissa Ghera, Ph.D.:** the things you just outlined. Right? Like, I'm not actually moving time blocks. I'm putting them in where we are. Tell me what classes you want somewhat, because we also have these pathways. So, like, for fall, I need to schedule the classes that are on the pathways. They need to be on the schedule. These are the time blocks that are well orchestrated and fit and are relatively well spread out. Now, who teaches those classes that I don't really care about? Like, that's the preference component. Right?

    **Adam Pryor:** Like,

    **Melissa Ghera, Ph.D.:** I need these 560 classes, or actually 650 classes, because they're on the pathways. They fit the curriculum that we have ordained, and they generally fit in these time blocks relatively spread out. Who goes into what slots? I don't

    **Adam Pryor:** got it. Okay, so you don't need this step at all.

    **Melissa Ghera, Ph.D.:** I. That I got a little lost on this one because I was like, I'm. I'm a little confused as to what the preference. I

    **Adam Pryor:** mean, what I would say is, like, fine. Like, again, this is just clarifying the sort of, like, process that you all have in place that I can kind of get a hold of it. Right. So. Right. If anything, the only thing that you would need out of this is are there ways that we can better optimize what's going on here based on the students we have at the particular time. Time. But that's a project that's a. That's not looking back, that's looking forward. Right. In terms of what you could. Like, you have a good system set up. You don't care who teaches in what block. And frankly, that's kind of the last thing to get filled in anyway.

    **Bethzaida Sosa (SJF):** So.

    **Adam Pryor:** I

    **Melissa Ghera, Ph.D.:** mean, faculty care. But like, from where I sit, like, I'll

    **Adam Pryor:** put in, tell

    **Melissa Ghera, Ph.D.:** me

    **Adam Pryor:** is teaching

    **Melissa Ghera, Ph.D.:** wherever. Like, that's not a. Right.

    **Adam Pryor:** So, so essentially, how. How fixed is your blocking system? Like, how. How confident are you that you go, I could give that to you in full. And for how many semesters?

    **Melissa Ghera, Ph.D.:** Right now, I'd say about 60%.

    **Adam Pryor:** I think we're

    **Melissa Ghera, Ph.D.:** working to a place where I will feel even more confident with that after this next fall.

    **Adam Pryor:** Got it. Do you need anything from an analytics perspective in order to take the next steps with that process? So

    **Melissa Ghera, Ph.D.:** what I think would be helpful, and I think it's on here somewhere. I think it might be number five. This

    **Bethzaida Sosa (SJF):** one.

    **Melissa Ghera, Ph.D.:** Yes. Maybe it's. Maybe it's. That one is to really see with all of the curriculum and the courses is if we have things in conflict. That's where I think the current system we have starts to break down. Okay.

    **Adam Pryor:** Because

    **Melissa Ghera, Ph.D.:** we have multiple divisions and people who don't check, cross check. And I'm one human. Yes. So,

    **Bethzaida Sosa (SJF):** Melissa, which one is it? So I didn't capture a lot of details for the predictive demand versus the conflict. Right. So

    **Melissa Ghera, Ph.D.:** it's more so the. I don't know where it is on here, but basically, like. So one conflict that I know. I'll do a. Say it by example. We can see where we caught it in here

    **Bethzaida Sosa (SJF):** is

    **Melissa Ghera, Ph.D.:** that there are. There have been multiple semesters, for example, where Organic Chemistry 2 is running at the same time as calculus.

    **Adam Pryor:** Okay.

    **Melissa Ghera, Ph.D.:** And those students need to take that.

    **Adam Pryor:** Yeah. Right.

    **Melissa Ghera, Ph.D.:** So. And just because one faculty member taught it and it got flopped to one hour later. Right. Like that type of conflict.

    **Adam Pryor:** Right.

    **Melissa Ghera, Ph.D.:** So if we could run the required courses in one semester with the required courses in other curriculum to make sure that they're not overlapping in the same time blocks. That's where my brain sometimes not breaks. I just miss things.

    **Adam Pryor:** Well, anybody. That's. That's totally fine. How. What are the cycles of your course teaching two year, three year. How often do courses

    **Melissa Ghera, Ph.D.:** come

    **Adam Pryor:** up? It

    **Melissa Ghera, Ph.D.:** depends on the program. The ones that are most problematic are probably chemistry because they have some of those small courses that are every third semester. Okay.

    **Adam Pryor:** And

    **Melissa Ghera, Ph.D.:** those are the ones that start to cause problems like P Chem. Acem.

    **Adam Pryor:** Yeah.

    **Melissa Ghera, Ph.D.:** It's a relatively small standalone major. Yeah.

    **Adam Pryor:** But

    **Melissa Ghera, Ph.D.:** it's

    **Adam Pryor:** required

    **Melissa Ghera, Ph.D.:** for lots of other things, you know, and they're with

    **Adam Pryor:** a ton of

    **Melissa Ghera, Ph.D.:** like

    **Adam Pryor:** required course. Yeah. Interactions. Yeah. How many of those things are mapped out? They.

    **Melissa Ghera, Ph.D.:** I don't have a good map. The chair will tell you they have a map, but I don't see it and therefore I'm relying on the chair and I have some control issues. So I totally admit that in this space. Well,

    **Adam Pryor:** let's look. It

    **Melissa Ghera, Ph.D.:** would be helpful if I had the map. Let's

    **Adam Pryor:** just assume the chair's lying. The map doesn't exist. The map is in their head. Nobody's actually ever written it down would be my guess. So. Okay, so if I went through, for instance, department by department, just

    **Melissa Ghera, Ph.D.:** for,

    **Adam Pryor:** for an example. Right. I probably wouldn't find a two year, three year, three semester, take your pick. Rotation schedule for an optimal, say four year graduation plan.

    **Melissa Ghera, Ph.D.:** Some of probably not. Well, Biology might have it. Biology might.

    **Adam Pryor:** Departments that definitely won't have it though. Correct.

    **Melissa Ghera, Ph.D.:** Okay,

    **Adam Pryor:** that's actually so like when I'm thinking about designing like an AI tool for that. Right. Like that's actually the base data you're going to need in order to build that tool. So like step one is going to be like, we're going to have to gather that if this is what we want to build. Right. So I'm just. Right. I'm poking at getting to a sense of like what already exists and what doesn't in terms of doing this. Okay, that's helpful. Can I ask some questions now beside. Or do you have

    **Bethzaida Sosa (SJF):** one? Absolutely. This meeting is for you to talk to Jason and Melissa directly and me not playing middleman. So. Yes. Okay.

    **Adam Pryor:** Jason,

    **Bethzaida Sosa (SJF):** walk

    **Adam Pryor:** me through how you build a catalog. We. I've seen the XML files, so I'm. I'm kind of guessing at some things, but I want to hear you run it

    **jwelch:** out. So there's kind of two. The, the course process and the curricular process are kind of two different processes. Okay. So you almost kind of have to follow those two things in their own separate thing. Yeah.

    **Adam Pryor:** Okay.

    **jwelch:** And then we, we reconcile those things kind of manually. So the course change process, you. We have an electronic form that goes through a workflow, gets everybody's approval ends up in the registrar's office. And not all of them directly impact program requirements. Some of them could just be like an open ended elective. But regardless, it follows the same process.

    **Adam Pryor:** Come

    **jwelch:** to the registrar's office. We create it in Banner. Okay. You know, if we have questions, that'll just become a standalone loop on whatever questions we're trying to resolve. Then once it's in banner, we run a query to export it out from banner and then oit imports it into WordPress for the catalog. Okay. And then all the while we're trying to reconcile that against the curricular proposals. So if Melissa sends me a curricular proposal and it has a course on it that's required for three credits and they made a mistake and submitted it for two credits, that's a problem. And so we try to reconcile those things.

    **Adam Pryor:** So

    **jwelch:** that's the course part. Okay. For the catalog itself part, it's basically a clone. And I think

    **Adam Pryor:** Kevin

    **jwelch:** mentioned he wants to change this. So I'll tell you how we used to do it and I don't know how we're going to do it in the future. Okay. We would send the links out to the departments. Okay. Pay close attention to places where we know that there was changes that went through curriculum. Get their feedback. Got

    **Adam Pryor:** it. And

    **jwelch:** then put it into WordPress and then get their feedback a second time that the thing that we gave them is what they wanted. Okay. And then in a perfect world, we've heard back from everybody with, yes, this is what I want. That doesn't always happen. And then we move forward with it.

    **Adam Pryor:** Oof. I'm sorry, that's a,

    **Bethzaida Sosa (SJF):** That's

    **Adam Pryor:** a brutal process.

    **jwelch:** Well, and you've heard Kevin say, like, why do the faculty have to be involved at all?

    **Adam Pryor:** Right. And

    **jwelch:** there's some gray area there.

    **Adam Pryor:** Well, yes, I. That's a lot of. Okay. And

    **jwelch:** actually, from my perspective, the biggest problem is that WordPress doesn't integrate with Banner by itself in any sort of way. So that when we do course change forms, we have to force those into WordPress and then figure out if we have a problem.

    **Adam Pryor:** Tell me about how you're forcing them into WordPress. That's

    **jwelch:** a Steve Vaughn question beside.

    **Adam Pryor:** Okay,

    **Bethzaida Sosa (SJF):** yeah, we can have.

    **jwelch:** It's an SQL to pull them out of WordPress and it's some sort of. Or it's an SQL to pull them out of Banner.

    **Bethzaida Sosa (SJF):** Banner

    **Adam Pryor:** and

    **jwelch:** then it's some sort of homegrown process to push it into WordPress. Yeah,

    **Bethzaida Sosa (SJF):** it's an extract and an end.

    **Adam Pryor:** Yeah, it's an extract transformation. Okay. And

    **jwelch:** it's a problematic process because it doesn't.

    **Bethzaida Sosa (SJF):** Yeah. It's always

    **jwelch:** capture

    **Bethzaida Sosa (SJF):** everything.

    **jwelch:** It's

    **Adam Pryor:** finicky. People

    **jwelch:** make mistakes

    **Bethzaida Sosa (SJF):** in

    **jwelch:** it. And it's the whole thing.

    **Adam Pryor:** Yeah. I mean, anytime you're going to do an etl, unless you've got those pipelines really smoothed out that you know exactly what's coming over each time. And if it's this old. Yeah.

    **Bethzaida Sosa (SJF):** From a catalog perspective and technology wise, that's the. That's the reason why we really need a catalog tool per se, because the one we have, it's. It's homegrown and it's unstable. Okay. And

    **jwelch:** Adam, can I ask you something maybe outside the scope of this, but from your experience? Yeah. In my opinion.

    **Adam Pryor:** This

    **jwelch:** is my opinion.

    **Adam Pryor:** If

    **jwelch:** you buy a catalog software, you. You really should have a curriculum software that integrates with that so that they feed off of one another. 100

    **Adam Pryor:** experience.

    **jwelch:** Yes.

    **Adam Pryor:** 100\. All

    **jwelch:** right.

    **Adam Pryor:** Convince

    **jwelch:** folks here that that's the.

    **Adam Pryor:** It makes zero sense.

    **Bethzaida Sosa (SJF):** I agree too. Right. You

    **Adam Pryor:** start at the source

    **Bethzaida Sosa (SJF):** and then feed the ultimate output. Yes.

    **Adam Pryor:** There is zero reason to do one without the other. If I will give you my very. I. I am not good at holding a poker face in any way, shape or form. Right. So that's why. It's why I choose clients very selectively. Right. Like, if you just do a catalog software. Right. Without the curricular pieces you're describing, you are going to have the exact same mess you have right now. And

    **Bethzaida Sosa (SJF):** the curricular pieces we're referring to is the curriculum

    **Adam Pryor:** tracking system

    **Bethzaida Sosa (SJF):** that

    **Adam Pryor:** it's running through start to finish. If you want to. If you really want to go that route. Right. That is a. That is a very holistic. And I love it. Right. I've. I've seen institutions implement that. Great. It is a wild culture shift from what you are describing in terms of how people think about tracking things through the process. Okay. So that. Agreed.

    **jwelch:** I just wanted to check myself to make sure I wasn't

    **Adam Pryor:** the crazy

    **jwelch:** one. As I've been harping on this drum for.

    **Adam Pryor:** No, you're not. You're not the crazy one. I will say it's doing both of those things together where these softwares get so pricey. Right. And I think that's the. That's the trick that I, you know, I'm not in the budget, so I don't know how that would. How well that would go. Yeah.

    **jwelch:** Tell

    **Adam Pryor:** me a little bit about. And I guess just to get us all on the same page. Right. Like when I'm talking About this, I'm thinking I keep using some of these terms in shorthand with the site up kind of back and forth. An ETL is just an extraction, transformation and load, which is to say you're going to take it out of one place with something like a SQL query, you're going to transform it in some way so it shows up someplace else and then you're going to load it up. Right. And so this was a very classic like model for computer Systems for about 30 years and is still used in a lot of cases today. So it's not like antiquated in that sense. Like people use this, it requires maintenance. And what I'm getting a good sense of from talking to you all is that the maintenance is so far out of date that things are getting to be problematically manual. So, Melissa, tell me a little bit about, tell me a little bit about how I'm trying to think, how to gently phrase this question, how it is in a, in a long term system that you would come out of a project like this and go, this was worth it. What do you need in, in, let's say just realistically, because we're now in November, let's say next fall,

    **Melissa Ghera, Ph.D.:** what

    **Adam Pryor:** do you need to have in your hand to go? This would have been, this would have been worth it for me.

    **Melissa Ghera, Ph.D.:** This system meaning an AI initiative or a cat, like a system purchasing initiative. What's the target we're shooting to? You

    **Adam Pryor:** choose. I

    **Melissa Ghera, Ph.D.:** mean, I think overall from where I sit, the goal of the exercise, right. Is to have a more, let me rephrase it, a less work intensive schedule process.

    **Adam Pryor:** Okay?

    **Melissa Ghera, Ph.D.:** Right. This is not hard. This is not rocket science. It's a little bit of a logic project that should go much smoother and quicker and should roll more easily. Right. It should be, in my opinion, something where even for a school like Arts and Sciences on a campus the size of Fisher, where there is some way to check, cross check requirements for curriculum, housing, room, assignment, spaces and faculty load and make sure that. And the number of seats for majors, the number of designated majors in a program and make sure that all of those things, check, cross check and are on the schedule. This does not seem like a horribly convoluted logic problem. However, when it is a human doing it right, it is laborious just because it's part of my job.

    **Adam Pryor:** Right.

    **Melissa Ghera, Ph.D.:** Somewhat fun because I am dorky like that. Right. But it just leaves room for error. Yeah.

    **Adam Pryor:** And

    **Melissa Ghera, Ph.D.:** unfortunately the error comes at the cost of the students. Right.

    **Adam Pryor:** And

    **Melissa Ghera, Ph.D.:** like that's the baseline that I feel like, has to be eliminated. Okay. Right. If the baseline is like, it's scheduled at the wrong time, but students can still take it, but it irritates faculty. Sorry, somebody else needed to check that behind me, you know, but the class getting taught and the students getting what they need. Okay.

    **Adam Pryor:** If

    **Melissa Ghera, Ph.D.:** the class is being offered and it's in the right curriculum and the students can progress, but it's conflicting with another required course, that's a major problem because now we're holding up student progression.

    **Adam Pryor:** Yep.

    **Melissa Ghera, Ph.D.:** So. Got

    **Adam Pryor:** it.

    **Melissa Ghera, Ph.D.:** The outcome of this is that we can have a schedule that students can progress through in a timely fashion to complete their major. And it's buys back some time and frustration. That to me, is a win.

    **Adam Pryor:** How many? Okay, I'm gonna. I'm gonna eliminate the graduate program for a minute because in a lot of ways that feels like a totally separate conundrum. It's not right. But I think you understand what I'm saying. How many majors?

    **Melissa Ghera, Ph.D.:** So we bring into Fisher? Like, our entering cohort is 650 students. Okay.

    **Adam Pryor:** In

    **Melissa Ghera, Ph.D.:** the first year. Okay. University. How

    **Adam Pryor:** many majors do you offer? Majors Minus.

    **Melissa Ghera, Ph.D.:** We offer. Well, the school of arts and sciences has about 28. Okay.

    **Adam Pryor:** Give

    **Melissa Ghera, Ph.D.:** or take. You know, some are. Some are still there, but very, very quiet, you know, so I'm gonna go with. I

    **Adam Pryor:** gotcha. Yeah, but. But I'm just. I'm.

    **Melissa Ghera, Ph.D.:** And then we have business and nursing and education. Right. So

    **Adam Pryor:** business.

    **Melissa Ghera, Ph.D.:** Three

    **Adam Pryor:** professional schools.

    **Melissa Ghera, Ph.D.:** Yeah. And three professionals. Well, in pharmacy. But they're mostly graduate.

    **Adam Pryor:** But they're mostly graduate from what I can tell. Right. Okay. Yeah,

    **Melissa Ghera, Ph.D.:** but like for our entering first year students, our center for career and academic performance, and myself, line by line cohort, A curated schedule for every entering student.

    **Adam Pryor:** No, I

    **Melissa Ghera, Ph.D.:** have built cohorts. Right. For the nursing students, the bio chem students, the bio straight students who take a different set of courses.

    **Adam Pryor:** Got it.

    **Melissa Ghera, Ph.D.:** And then the main programs. So I have built a schedule there. All their main required courses go together. Yep.

    **Adam Pryor:** And

    **Melissa Ghera, Ph.D.:** then line by line, each of those students is entered in. So we've got to the point where I've gotten the main courses to go together. Like nursing, for example, takes anatomy. Anatomy, Anatomy, Physiology, Anatomy, physiology lab, their nursing seminar, and our learning communities. Right. So I've built a schedule where all of those things are not in conflict. Correct.

    **Adam Pryor:** I'm

    **Melissa Ghera, Ph.D.:** hoping that this fall we can just rinse and repeat that to the next fall. Right. That's 150 students.

    **Adam Pryor:** Yeah. You

    **Melissa Ghera, Ph.D.:** know, and then accounting is macro or Micro and accounting one. And their business course. And I've built 160 lines of that. Okay.

    **Adam Pryor:** And

    **Melissa Ghera, Ph.D.:** then so on and so forth. Right. So like I have line by Line built 600 lines of classes that fit together. So for 80% of that, it's solid. But when people want to teach over here or want to teach over there or want to teach and it doesn't go together, like, that's where we run into difficulty. Right. And it's ultimately at the cost of. Yeah,

    **Adam Pryor:** we

    **Melissa Ghera, Ph.D.:** don't want it to be the cost of the student. Okay,

    **Adam Pryor:** so whose job is it to tell that faculty member you can't teach them? Okay, got it.

    **Melissa Ghera, Ph.D.:** Yeah.

    **Adam Pryor:** Okay. So, Jason, what do you need? Just

    **jwelch:** a follow up.

    **Bethzaida Sosa (SJF):** Is that,

    **jwelch:** is that possible? What Melissa was just describing, do you think would an AI bot be helpful in that?

    **Adam Pryor:** Oh, I mean, I think an AI bot would be immensely helpful in that, frankly, if for no other reason than what you could do. Like, look, just sitting and talking with you all today, right? Like, here's what I would. Here's how I would build something like that, right. One, it's not for the students, it's for you all.

    **Bethzaida Sosa (SJF):** Two,

    **Adam Pryor:** what you would need, and this is why I'm sort of poking at some of the things I'm poking at. You need a good solid list of all of the courses that you could trust that you know that that's there. You would need four year plans for an idealized schedule. Right. For a graduating student. Right. And then you would need course rotation schedules. In the fall of an even year, we teach this. In the spring of an odd year, we teach this. When you have those three pieces of data scheduled together, you can create or at least have a check for the work that Melissa's already done. Right. So she's already done a ton of handwork. I don't want to like repeat that. But you could absolutely run those into a clean system. Ask it to look for conflicts. Right. If you've flagged the data the right way and then have it, you know, spit it out, frankly, an AI system is really great for that because it can do a little bit of the interpretation for you so you don't have to hard code everything in. That's a you. Ideally, you could program that and you wouldn't need AI at all. But the reality is it would break, it would be really, really brittle and it wouldn't. It would, you would really struggle. I say all of that with the giant caveat to say if there's not somebody on the back end of that, who is going to hold the stick to the Faculty and say, you must teach at this time. For that reason. It won't work. You'll build a beautiful, idealized system that won't do what you need it to do. So, yeah, I look at that and go, like, it's totally possible. It's, it's. I mean, it's not a small project, mostly because what you actually need to do it is a series of interviews with people to pull information out of their heads, unless they've all got it written down already. But I've never worked at a campus where that was the case. You know, it's gathering those pieces that. That's really, really critical. But that's not. That's not a catalog project. I. I mean, really. Right. That's. Yeah.

    **Bethzaida Sosa (SJF):** So, Adam, this started off as a catalog project. Yeah.

    **Adam Pryor:** It's clearly not. I'm fine with that.

    **Bethzaida Sosa (SJF):** Yeah, it's.

    **Adam Pryor:** Yeah, I think

    **Bethzaida Sosa (SJF):** catalog

    **Adam Pryor:** was

    **Bethzaida Sosa (SJF):** one of the. Yeah.

    **Adam Pryor:** I just want to. I just want to make sure that I'm like, kind of going to things that are actually going to help. But, Jason, I mean, to answer your question in the short, it's. It's yes and no. Like, we could build it. You could use AI to help. You could do it in a hurry. I don't have any doubt about that. And what the AI is going to do is do some of the transformational pieces that we're describing in a current workflow, like what you have, hopefully without it breaking every time. That. That would be the measure of the success, or breaking a lot less is usually what I like to say when I'm working with AI stuff. But what do you need at the, at the sort of end of this to make it worth your time? Well,

    **jwelch:** I mean, I've been harping on the curriculum and catalog because our process is so outdated.

    **Adam Pryor:** Well, the result of that is it's manual on you.

    **jwelch:** Yeah,

    **Adam Pryor:** yeah. Let's just. Yeah, yeah.

    **jwelch:** So, I mean, if. So if we put that aside, because that's really. I mean, a dedicated software conversation. If we put that aside, then something helpful would be if AI could insert itself on the course change process. Okay. To fact check. Like, because presumably this AI bot would know our catalog and could

    **Adam Pryor:** presumably

    **jwelch:** know and look at our curricular proposals. Yes. So those, Those proposals and that process is disjointed from the course creation process.

    **Adam Pryor:** And

    **jwelch:** Melissa tries to insert herself in that and ask questions where appropriate, but things fall through the cracks. So, you know, would a bot be able to insert itself into that process to. To fact check those course changes against. Yeah. Slash catalog.

    **Adam Pryor:** Yes. The. The short answer there is yes, we could. We could design something like that. So

    **Bethzaida Sosa (SJF):** there was this other request. Jason. I mean, Adam. Yeah. Melissa. Right. Recommended. Asked if there could be a system or AI bot to help run B data or draft schedules to help produce recommendations for conflicts with classrooms. Yeah,

    **Melissa Ghera, Ph.D.:** I think that goes into that whole.

    **Bethzaida Sosa (SJF):** I was. I was trying to figure out how. Like,

    **Melissa Ghera, Ph.D.:** I thought we had it on here somewhere, but I

    **Bethzaida Sosa (SJF):** think it

    **Melissa Ghera, Ph.D.:** was down where I couldn't see. Yeah,

    **Adam Pryor:** yeah, yeah, yeah, yeah. That's. That's essentially a touch.

    **Bethzaida Sosa (SJF):** So I think these two might go together. Yeah. So, yeah,

    **jwelch:** that's just a little bit more

    **Bethzaida Sosa (SJF):** detail. Like,

    **jwelch:** tell me where I have too many seats popping possibly because the last five. Tell

    **Melissa Ghera, Ph.D.:** me where Cal and Orgo two are in conflict and where they're. You know, you

    **Adam Pryor:** could. And you could kind of do it in a double way. Right? Like you could imagine a couple of fake students and see where they're like. And mock their enrollment out of it, actually. And then you could also do the. The conflict checking piece. Yeah, that. That would be. That would be feasible. Okay, so it sounds like. All right, well, now I'm gonna. Cone of silence, right? You're

    **Melissa Ghera, Ph.D.:** an outtaker. That's on. Not ours. Yeah,

    **Adam Pryor:** I know, but I'm not giving the notes. Cone of silence. When it gets down to it, you all are probably the people that I'm working with to do this, maybe a couple of others. Right? But. But

    **Bethzaida Sosa (SJF):** yes, nitty

    **Adam Pryor:** gritty. You all are the people who are actually going to make this happen or not happen. Okay, great. There

    **Bethzaida Sosa (SJF):** might. There will be a few other Melissas based on the score.

    **Adam Pryor:** Yeah. Oh, absolutely. Absolutely. There's

    **jwelch:** only one Melissa.

    **Adam Pryor:** Insulting.

    **Bethzaida Sosa (SJF):** Sorry. So we're

    **Adam Pryor:** gonna call them Melissa, Beta, Gamma and Delta because they're not as good. No

    **Bethzaida Sosa (SJF):** other schools have the same role that Melissa has. That would. Yes,

    **Melissa Ghera, Ph.D.:** there are four of me. Four more.

    **Adam Pryor:** God

    **Melissa Ghera, Ph.D.:** help

    **Adam Pryor:** us. But

    **Bethzaida Sosa (SJF):** she has the largest school with the largest change rate and the largest amount of. And arts and sciences has. Is the school that has the most cross. Right. You've

    **Adam Pryor:** got the most. You've got the most at stake in other

    **Bethzaida Sosa (SJF):** integration along with other schools. Yeah,

    **Adam Pryor:** you're gonna have to. You're going to. You're going to have your fingers in everybody else. Yeah. So this is what I would like to. To recommend. I am working on sort of re. Amending the project proposal. Right. I'm going to strip it way down. That's what I'm doing. I'm not. There are still. There are at least the number of bots that I was previously envisioning. They're just variations on what's going on here. The scope of the work beside just for. For anything you would want to tell Chris or something like that, the scope of the work I'm going to propose isn't going to change. That's all going to look exactly the same. I can work with that. And this is interesting to me, so this is helpful. I'm going to attempt. I have to talk to the cabinet on Monday. So between now and Monday, in my infinite free time, I want to. I want to do a couple of things. I want to try and put forward a proposal that speaks to the items that are important to you and I'm going to try and recap those before we leave so that I feel like I've got a good handle on representing some of the things you all said today. And I'm going to just flat out make some recommendations out of the get go about how I would do this to them that not all of which they're going to like and I will take the heat for that or they just won't hire me. And that's okay. But it also then gives, I think, a way to voice some of the things you all are saying and aren't being heard. Right. And that to me is really, really important. So one is on the catalog piece, Jason, you need to be set up so that it is built into the budget at some point that there is a curricular and a course structure to the piece that you would add on with a software. And they need to be thinking about that in the same way they would think about an lms. Right. You're going to eliminate eventually and I don't know when they're going to want to do this, but you would eliminate the processes that you are going through right now because you would have something that has a direct feed to the API system and Banner. You don't even need to know everything that that means.

    **Bethzaida Sosa (SJF):** But

    **Adam Pryor:** hear me say that's course dog in a nutshell. Okay. You would eliminate this process of you writing a SQL query, handing it off to someone and then having it transformed. Instead, you would layer something directly on top of Banner that everyone would have access to. And instead of doing this by paper, they would upload their curricular changes to that system so they're being tracked automatically. That

    **jwelch:** is my goal. There

    **Adam Pryor:** you go. Okay.

    **jwelch:** Been getting folks on board with that quite yet. But yeah,

    **Adam Pryor:** so that to me is like, let's, let's. We're going to call that Kind of the gold standard to say like that. That makes sense. That's the right thing to ask for. And when we're talking about doing the. The rfp, that's what that RFP needs to be shooting toward. Yeah.

    **Bethzaida Sosa (SJF):** So, Adam, did I hear correctly that the recommendation would be to update Banner directly? No,

    **Adam Pryor:** no, no, no. What's your. What's your lms? You guys use Canvas, right?

    **Bethzaida Sosa (SJF):** LMS is brightspace.

    **jwelch:** Brightspace.

    **Adam Pryor:** Brightspace, okay.

    **jwelch:** You're

    **Adam Pryor:** going to think of whatever program you use as the equivalent of Brightspace, right? I'm assuming your BrightSpace is pulling information from an API out of Banner. Yeah,

    **jwelch:** it is.

    **Adam Pryor:** Okay. You're going to, you're going to think of this as the same way. It's a. It's a software that you're going to layer on top. Okay.

    **Bethzaida Sosa (SJF):** Totally.

    **Adam Pryor:** Totally typical solution.

    **jwelch:** And many, many schools do this, Adam. So

    **Adam Pryor:** you're

    **jwelch:** not

    **Adam Pryor:** crazy.

    **jwelch:** I mean, I don't think that you and I are crazy for.

    **Adam Pryor:** No, no, no, no, no, no. What's. What's hard about it, Jason, just, just. And I'm sure you have experienced this too, is that finding a halfway point between those two things, all on paper or moving to this system, starts to break down. And so it's hard to implement in. In phases in my experience. Like, it's. It's a little better to just rip the bandaid off and go after it. Okay, so that's one, two is then to say. Let's imagine that there is going to be some time in between this. And I'll be blunt, I don't trust wrappers. Wrappers are what we call AI systems that are built on top of other systems. Right. So Banner will have one, but BrightSpace, I'm sure BrightSpace has developed something where they've got AI turned on. Right. And AI will do this for you inside of.

    **Bethzaida Sosa (SJF):** Yes. Within the environment? Yes. Yeah.

    **Adam Pryor:** Canvas has one. Hear me say they tend to be pretty useless. And the reason they're useless is that you don't know the instructions and you don't know the language model that they are using for those instructions. And they tend to be pretty superficial because that's what they have to do in order to scale it to the wide variety of institutions that it would be useful to. So, for instance, what you're asking for, Melissa, I don't care who tells you they can do it with AI, it's going to break. It's not going to work. And the reason it's not going to work is unless they custom build it off of your Data, it's not going to do what you're asking it to do. And I don't know of any large language model that you would be able to upload that data smoothly without some significant transformations. And it would do that. And if they're telling you it will, they're lying or they're not understanding what you're asking for. Full, full stop. I can say that with confidence. There is only one outside external company that I would recommend that could do that for you and would, would promise to be able to do it across scale. Like it would integrate directly with information being pulled from Banner and could then integrate with other foundational systems. That company is called Dewey. The average implementation cost for Dewey for one module, right. Just to pull things from Banner, it would ignore Brightspace or something like that entirely. Is $80,000 minimum for the initial setup plus 6.

    **Bethzaida Sosa (SJF):** And that's for what exactly which, which process you're referring to.

    **Adam Pryor:** It would be so on the AI side beside it, somebody who is saying we're going to create an in house data lake. Yeah, right, like that. That you and I know the only way to solve the problem that Melissa is describing in the long term would be to build an in house data lake. And I could be wrong, you could tell me I'm wrong. But there is nothing you have told me that says you guys are ready or, or able to do that yet. And you could bring in somebody from the outside to do it. But I mean that, that pretty quickly starts to look like an implementation project. That's a small scale sis. I mean it's, it is not a small. If that is what you wanted, I would happily give you recommendations for people to talk to because that's on me. Right. What we can do though is essentially build a black box system because you're small. Right. And what's going to go away from this and what I'm going to kind of put on the shelf is a little bit of the, a little bit of the predictive analysis. I'm gonna, I'm gonna box that for a second because I think you could get about 85 to 90% of the. Where you wanna go just on a descriptive analysis, right. Which is to say I would wanna gather together those core data sources and clean them and hold on to them so that we could run a test. What the ongoing maintenance of that would be is updating them on a yearly basis and I think you could match that against the catalog.

    **jwelch:** And by updating them you're talking about basically like a pathway. Yeah,

    **Adam Pryor:** I'm Talking about a pathway, when it gets down to it, it would have to be a custom built pathway. And I'm not in favor of that generally, but I do think it is a holdover that you could use. It would probably serve you well for the better part of five to 10 years. I like that timeline because AI is also the Wild west. And there is a distinct possibility that what you would build today anyway is going to be outmoded by five to 10 years. But it will also set you up to be able to do that going down the line. Does that make sense? Kind of in a. In a basic way. I'm going to orient what we do around the sort of two outcomes you all described. Right. That. Jason, you need an RFP that leads you towards this other direction. I don't know what the timetable of that looks like. Melissa, you need a system that allows you to do this kind of checking and allows the other deans to do this kind of checking. But it comes with some change management about what authority is going to be given to people to implement this system and keep it consistent. And that is part of where the original plan was for me to do some work on strategic planning around AI. I'm going to include that kind of in there. How Essentially I'll. I'll draft out a model of how do you build a tool, but then it fails. And what are the pitfalls you're going to need to avoid in order to make that the case? Spoiler. Faculty are going to hate it.

    **Bethzaida Sosa (SJF):** Why do you say that? I just want to understand your thoughts.

    **Adam Pryor:** Melissa understands exactly what I mean. We're going to take away some of their autonomy out of doing this. They're no longer going to be in their own little fiefdoms. And that sounds like it won't be a problem. This is a. The faculty always work on the 8020 rule. For 80% of them, this is not going to be an issue at all.

    **Bethzaida Sosa (SJF):** But

    **Adam Pryor:** for the 20% for whom it's going to be a problem, they are going to be loud about it.

    **Melissa Ghera, Ph.D.:** Be a big problem. Yeah.

    **Adam Pryor:** Yes. And they're going to. And they're going to try and make it everybody else's problem. So some of this is also going to be to figure out what kind of real change management is going to need to be put in

    **Bethzaida Sosa (SJF):** place

    **Adam Pryor:** in order to make these systems work as you're going through. Right. So we need demonstrable test cases that are going to create campus buy in as part of doing this.

    **Bethzaida Sosa (SJF):** Yeah. So, Adam, the. The tools you're Referring to would be tools that Melissa would use, but

    **Adam Pryor:** the

    **Bethzaida Sosa (SJF):** Melissa

    **Adam Pryor:** and her.

    **Bethzaida Sosa (SJF):** And the results will impact faculty in terms of their schedule

    **Adam Pryor:** or preferences

    **Bethzaida Sosa (SJF):** or whatever. There

    **Adam Pryor:** are tools Jason use also, but in a much more straightforward way. Right. So, Jason, I'm. I'm just going to imagine, I think you have probably been preaching the good news and I don't think people understand when it gets down to it. So I'm. I'm just a very practical person who thinks that's going to slow down the timeline of how that's going to get implemented. And I want to try and create systems that are going to do two things. One that will make that shift over easier

    **Bethzaida Sosa (SJF):** and

    **Adam Pryor:** two that are going to try and make some of what you are doing less manual. And I'm going to have to.

    **jwelch:** Yeah, I don't really know. Maybe I

    **Adam Pryor:** done

    **jwelch:** a poor job on trying to get everybody on board with this. I don't really know. I had a half a thought to pay beside under the table to break WordPress entirely. So

    **Adam Pryor:** we had

    **jwelch:** to do something different.

    **Bethzaida Sosa (SJF):** So that's

    **jwelch:** still. I'm going to fall back to that.

    **Adam Pryor:** I like your plans. I like your plan. Yeah. So,

    **Bethzaida Sosa (SJF):** I mean, I think one of the things is Jose's on board. Right. So I think we're slowly getting there. And I think this project, even though it's been a bit of a turmoil and a lot of active conversation, I think it's a good thing because it's getting people to listen. And secondly, it's starting to get people at different levels to dig deeper and truly understand the processes. I think that there's still more exercises to go through with Cabinet. And specifically I think Jose is. Gets it a little bit more. I think there's more conversation that has to be had with Kevin to understand.

    **jwelch:** Yeah. But I don't understand is Kevin is not in support of a curricular piece of a software. And then he'll bring up the fact that it takes 18 months to complete that.

    **Bethzaida Sosa (SJF):** Yeah.

    **jwelch:** And that's why he doesn't want to do it. And I don't understand that because what I hear is the process is very laborious and it takes a long time and we should try to do something different to make it better.

    **Bethzaida Sosa (SJF):** Yeah. So Jason and Melissa, what I want to do is schedule a session with Kevin and Amy and the three of us at minimum walk through those process maps with them, because we didn't do that. Right. So all of these conversations are taking place based upon not understanding what's under the hood and that there, there's a disconnect in the conversation and understanding. Okay, but I've digressed. We'll do that,

    **Adam Pryor:** but

    **Bethzaida Sosa (SJF):** go ahead, Adam.

    **Adam Pryor:** I, I think there are probably. You'll also find out I'm just kind of like a run ahead kind of guy. So we're just gonna, we're just gonna run ahead with a couple of things.

    **Bethzaida Sosa (SJF):** I'm

    **Adam Pryor:** gonna, I, I'm gonna call a colleague of mine because I want to ask some questions to a friend that I have about some of those change management pieces. That's not my area of specialization, but I, I know some people who do specialize in that. And I want to think about that a little bit more in part because any flack that comes back out of something like this should come back to me, not to you all. And that's. I want to, I want to make sure that that's the case. I want to think about that interim period. Realistically. You do an rfp. You start it now, you put it out there, you bid it out, you select something you want your start date for. Something like that is going to be fall 27. And that's a nothing goes wrong timeline. Right. So if we're, if we're shooting for fall 27 for that, to my mind, you've got this sort of 18 month window to say how much can we clean up and get ready for that to start before, before they start, you know, really working on it. Some of it you're going to do while they're there. Right. But we can, we can get this going. This is going to sound silly, but I think it's actually going to help Jason tremendously. And Melissa, it's something we'll have to roll out to the chairs. Your catalog's ugly. That's nobody's fault. You can see that it's been, you know, accreted over such a long period of time that nothing looks similar anymore. We need some templates. Sounds very basic, but like, every department should look the same. I don't care how special you think you are. We should have formatted places where there is a overview and there is a department contact and there are courses and these are formatted in very particular ways. So that this is essentially you're turning the catalog into a handbook. Now. You don't have to do that with the front matter. That's a, like a separate thing. But in the short term, Jason, I think it would be helpful for you, as we're doing the RFP process, to imagine what you want the catalog to look like. For instance, with like A course dog. And I'm just using them to say like it's a familiar one that people tend to know and

    **Bethzaida Sosa (SJF):** kind

    **Adam Pryor:** of envision what it looks like. Right. Like you want to set up a catalog that looks like you could copy and paste pieces of that into the structure of the system that they have because it's going to make the implementation of that easier down the road.

    **jwelch:** A lot of

    **Adam Pryor:** the,

    **jwelch:** the way that courses tie to programs in the current catalog are limitations in WordPress. Yeah.

    **Adam Pryor:** That

    **jwelch:** we mask

    **Bethzaida Sosa (SJF):** over time.

    **jwelch:** Yeah.

    **Adam Pryor:** And I, what I'm looking at, I can kind of see that in how the XML is structured.

    **Bethzaida Sosa (SJF):** Like

    **Adam Pryor:** I was, I was kind of getting the sense that that was what was going on. It's

    **jwelch:** actually a big problem and it's more of a problem the more cross permutations of programs that Melissa comes up with, with bringing in different subjects.

    **Adam Pryor:** Yeah, oh, absolutely. It's a problem, actually

    **jwelch:** a really big

    **Adam Pryor:** problem

    **jwelch:** that

    **Adam Pryor:** we've

    **jwelch:** been trying to solve in WordPress.

    **Bethzaida Sosa (SJF):** And as we're talking, what I'm also thinking is as we go through an RFP process and these tools, these AI tools that we're building can help get us to a better state over the course of one to two years. Right. And then maybe we have to focus on a module for the catalog and then do other modules as time goes on because we've built a process that has at least simplified it enough to sustain for a period of time. Yeah,

    **Adam Pryor:** you might, you might. I'm

    **Bethzaida Sosa (SJF):** just thinking where, where the largest pain point is and the risk, the

    **Adam Pryor:** largest

    **Bethzaida Sosa (SJF):** risk is with the system itself for the catalog production. Okay,

    **Adam Pryor:** so let's look at it this way then, Melissa. It's going to be helpful for me to sort of see your 600 lines. Are you okay sharing that with me? I just, I. It's probably the most comprehensive document from what you've described on the campus for how that's occurring now. And so I just, if I can sort of start to wrap my head around it. No, I'm going to have to ask you questions. But I, I think I have a good sense of what you were doing and why. And if I look at it, I think I'll have either more questions or be able to figure out what our next step is going to be. But to me, that's probably place one for you and Jason, I would like to run by what the template of those catalog pieces are going to look like going forward, Jason, what I'm going to have in mind and what's going to be helpful to me to have from you are what some of those SQL queries look like to pull the.

    **Bethzaida Sosa (SJF):** From my

    **Adam Pryor:** team

    **jwelch:** specifically.

    **Adam Pryor:** Not necessarily for.

    **jwelch:** For what we use to populate the catalog.

    **Adam Pryor:** Yeah.

    **jwelch:** Yeah. So the beside of that's one that Mark

    **Bethzaida Sosa (SJF):** runs

    **jwelch:** based on a view and then hands it to Steve.

    **Bethzaida Sosa (SJF):** Yeah, I would have to.

    **Adam Pryor:** Yeah. Okay. So beside that, that might be the next thing that I need are some of what those SQL queries look like. Um, so that maybe you and I can figure out a little bit of why the way the SQL query is structured is not loading more smoothly. And.

    **jwelch:** And I have a. The results of this SQL query in my. In my inbox somewhere beside it. But. Okay, it's a. It's an older one, I think,

    **Adam Pryor:** but I don't necessarily like. I don't need access to the system for any of that. Beside, I just. I think if we look at the SQL query, we can probably. Yeah,

    **Bethzaida Sosa (SJF):** we can

    **Adam Pryor:** send.

    **Bethzaida Sosa (SJF):** Sure.

    **Adam Pryor:** Yeah. Yeah, yeah. What's. Maybe what's holding it up? Because I think if we could get that smoothed out, at the very least you'll have a more efficient system for thinking through in the short term what's going on. Yeah.

    **jwelch:** Sometimes it's the issue with the query, but sometimes it's an issue with the load into WordPress.

    **Bethzaida Sosa (SJF):** It's the integration itself. And

    **Adam Pryor:** my guess is that it's. It's probably. I want to look at both because. But I want to start with the query to say is. Is the query. So

    **Bethzaida Sosa (SJF):** I can send you the query and then if you want to set up a

    **Adam Pryor:** quick

    **Bethzaida Sosa (SJF):** 30 minutes with my team, we can do that.

    **Adam Pryor:** Yeah, we can kind of like walk through that. That. That'll probably be the next helpful piece to sort of

    **Bethzaida Sosa (SJF):** play

    **Adam Pryor:** with. I will. I will share with Beth Seida and then I, I think probably the two of you all as well. I don't have any problem with that kind of what I'm suggesting based on this conversation. If you see something in it that you go that. That is not quite what we talked about or can we. Can we clarify this or. Or tweak that. I'll try and do it as quick as I can. It'll probably come to you over the weekend. Sorry. I'll

    **Bethzaida Sosa (SJF):** send you Jason and Melissa's emails because I don't think you. Yeah.

    **Adam Pryor:** And I'll add you guys to that piece so that you can see it and make sure I've reflected this as correctly as I can. This is super helpful. Thank you. I know we were like scheduled for 30 minutes and we took an hour, but I appreciate it. It will make this a little easier for me to sort of take that next step and how to, how to suggest what would come out of that. All right, I have to run to another meeting. This is what I do on Fridays, I've decided. But

    **Bethzaida Sosa (SJF):** so much for

    **Adam Pryor:** blocking

    **Bethzaida Sosa (SJF):** it off. Yeah,

    **Adam Pryor:** I appreciate it. I hope we will get to work together on moving this forward. I do think there's a lot that can be done, some of which can be up and rolling pretty quickly, some of which will take a little longer. But there's net benefit to have from continuing to move this forward. There's no doubt in my mind that there is labor to be saved out of organizing this, and I think that's a big piece to hold on to. All right, I will see you all.

    **jwelch:** Thank

    **Adam Pryor:** you

    **Bethzaida Sosa (SJF):** all. Thank

    **Melissa Ghera, Ph.D.:** you,

    **Bethzaida Sosa (SJF):** Jason. Bye. Bye.

    **jwelch:** All right. Bye.
