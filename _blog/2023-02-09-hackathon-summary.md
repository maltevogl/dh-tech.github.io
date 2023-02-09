---
layout: post
title: Join me for a DHTech hackathon? It’s an un-date!
date: 2023-02-09T10:00:00
tag: "WhatsHappening"
img: assets/images/posts/hackathon.jpeg
img-credits: Photo by <a href="https://unsplash.com/@pankajpatel?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Pankaj Patel</a> on <a href="https://unsplash.com/photos/_SgRNwAVNKw?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
author: Rebecca Sutton Koeser
excerpt: Rebecca reflects on the first DHTech Hackathon!
---

In November of last year, DHTech held our first hackathon. I wasn’t sure what to expect from it, but I was excited at the prospect of working on something with other members in the community and creating something together.

I’ve participated in hackathons before; I’ve even participated in some in-person hackathons, although not in a long time — certainly not since the pandemic, and probably not since I had children. Typical hackathons are notoriously unwelcoming in a lot of ways, including to people with care-giving responsibilities (but also often to non-developers or newer developers); the shift to “data jams”, as organized by Library of Congress or my former co-worker Nick Budak, are in part an attempt to address this problem.  I did recently participate in a virtual one-day hackathon organized by some IIIF folks to help work on the iiif-prezi3 python library, which was an interesting experience — I could tell the organizers had done a ton of work ahead of time to prepare tasks that were documented and could be picked up and worked on in parallel, but even with that preparation it was hard for them to keep up with answering questions and reviewing pull requests during the hackathon. Many of the contributions made during that one-day hackathon were not approved and merged into the codebase until long after the fact.

In this case, we couldn’t do that kind of preparation beforehand because we wanted to determine what to create and develop as a group. We knew from the sign up form that we wanted to focus on something related to fuzzy and uncertain dates, since that was the topic of most interest to everyone — and it’s something that has come up before during other DHTech meetup conversations as something that impacts many of our projects.  We kicked off the hackathon with a zoom meeting, and shared examples of some of the problems we wanted to solve or had run into in our various projects, similar projects and code libraries that might be relevant or good references, and even in some cases, code that some of us had created that might be related to the work we wanted to do. In my case, I  shared a link to the Shakespeare and Company Project codebase where I implemented logic for storing and reasoning with partially known dates (year, year/month, year/month/day, and month/day), and a link to the Princeton Geniza Project codebase where I have logic for converting dates from different calendars, leveraging the existing python `convertdate` library (a library I first learned about thanks to a DHTech member!).

In our kick-off meeting we brainstormed a list of tasks, but determined that first we needed someone to implement the initial data model — and decided that two of us (Cole Crawford and I) should find some time for pair-programming to tackle that task. Cole and I were able to find time later that afternoon to get started, and were able to get far enough to push code and create a pull request so we could get review and set the rest of the contributors up to start building out more functionality. (I think it was in this initial session that I came up with the provisional name “undate” for our new code library — I wanted something short, unique, and recognizable, and liked how the “un” gestures at the uncertainty and unknown or partially unknown dates that we want to be able to work with.)

There are a number of challenges involved in running a hackathon. In this case, there were logistical and practical difficulties as well as communication and collaboration challenges. Because DHTech members are currently spread out across the U.S. and Europe, **time zones** made it harder to schedule time together, and sometimes exacerbated the problem of **waiting for review** on pull requests.  **Time** was a challenge in another way, too — that is, finding and making time to work on the project. We scheduled the hackathon to run over an entire week, and we polled people for availability to try to find a good week to do it, but it seemed that most people were fitting it in around their other work commitments and busy schedules, which didn’t leave a lot of time for development work.  Other challenges related to **leadership** and **participation**. Because we didn’t have the work planned out in detail ahead of time, we hadn’t identified a person or group to lead the development. I took on a bit of an unofficial technical lead role because we were building on code I’ve written before and problems that I’ve been wrestling with for a long time, but maybe it would have been better if we’d designated a few people as official technical leads and empowered them more to make decisions and move things forward. I think the lack of planning ahead also made it harder for newer developers and less technical people to get involved. There were a couple of people who joined the kick-off meeting who didn’t end up participating, and I’m not sure if that was due to time constraints, interest, or a lack of easy ways to help. A smaller technical difficulty was reconciling differences in tooling and approaches (perhaps due to lack of clear leadership); this was an opportunity in a way, because we all got a chance to learn from each other about the different ways we’ve been doing things, but it also meant that we spent longer on setup tasks and infrastructure, leaving less time for tackling the real problems of working with uncertain dates. 

In spite of all these difficulties, the hackathon was also full of wonderful opportunities. I got the chance to do pair programming with people that I’ve never worked directly with — DHTech members and friends that I see regularly on Zoom but have never collaborated with. This should have been an opportunity for newer members to pair up with more experienced people; some of us offered times on Slack for just that, but it didn’t work out this time — and I hope we do better the next time. This is also an opportunity beyond the week of the hackathon: we’ve started developing a useful tool that many of us will be able to use across our projects. But it also occurred to me during the week of the hackathon, we can and should build it out so it is stable and feature complete so that we can submit it to the [Journal of Open Source Software](https://joss.theoj.org/) (JOSS) as a research software publication.  

This hackathon and the undate project is also a personal opportunity for me. I’ve been working with uncertain dates for some time now. It was relevant on both [Shakespeare and Company Project](https://shakespeareandco.princeton.edu/) (see my essay ["Coding with Unknowns"](https://cdh.princeton.edu/updates/2019/12/05/coding-unknowns/)) and [Princeton Geniza Project](https://geniza.princeton.edu/). During the week of the hackathon, I remembered that my work on this goes even further back, to a simple public domain checker I implemented for Emory University Libraries as part of a digitization workflow. I’ve been interested in generalizing this work and making it more reusable, but I don’t know if I would have found the time to do it on my own — and whatever I did wouldn’t have been as good without the input of collaborators and ideas about how the same or similar problems apply to other projects. 

What’s next?  Well, for me personally, I hope to find time to continue working on undate. I have lots of ideas about what else it needs and where it can go; you can see some of them in the [issues on GitHub](https://github.com/dh-tech/undate-python/issues). In the short term, I’d like to get to an alpha version published on PyPI. In the longer term, I want a stable, feature-complete version that people can start using for any python-based projects, and that we can submit to JOSS for review. As for DHTech — we’re talking about doing another hackathon. Maybe we’ll do another round of collaborating on undate; and if we do, this time we can plan ahead and hopefully make it easier for people to contribute. Or maybe we’ll pick a different topic or need within the community and start on a new tool. It could be that we’ll schedule an in-person hackathon at a conference, which would be a different dynamic entirely!  

Are you interested in contributing to undate? Are you interested in a future DHTech hackathon, either working on undate or something else? Or do you have ideas about how we can make it more welcoming and inclusive to any members in our community who want to participate? Please [join us on Slack](/join) or our next meetup and participate in the discussion as we think about next steps and possibilities.