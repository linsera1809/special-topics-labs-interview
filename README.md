# Interview time with Jeremy

## Overview
To give you a better idea of "real" GitHub workflows, I want you to fill out the below interview.  Many open source projects have their source repositories available publicly on GitHub.  They want to accept contributions from anyone, but they also have a few requirements:
1. They don't want to allow direct push access to their repository, because they want to choose whether or not to accept the patch (perhaps they need to require a license agreement, or they want to make sure all tests pass before taking the patch)
1. They want to be able to give feedback on the patch before accepting it (perhaps it violates coding standards, or is missing tests, etc.)

For git repositories with these types of requirements, GitHub has the [pull request](https://help.github.com/en/articles/about-pull-requests) process. Pull requests let a third party propopse a patch to the repository, and let reviewers (either human or machine) provide feedback and request additional changes for the patch. 

There are multiple ways to make a pull request.  For open source development, adding everyone who wants to send a pull request as a collaborator to that repository is infeasible (even if there are fine-grained permissions to allow for "pull-request-proposer only").  So their pull request model more generally follows this pattern:
1. User Bob wants to contribute to project `next-best-thing` (which is publicly available on GitHub).  User Nancy is a "maintainer" of `next-best-thing`.  That means that Nancy has the rights to modify the repo (merging commits, rebasing, etc.).
1. Bob starts by [making a fork](https://help.github.com/en/articles/fork-a-repo) of `next-best-thing`.  That means he has a copy of `next-best-thing` in his GitHub account, along with metadata that "remembers" that the original source of this repository was the authority `next-best-thing` maintained by Nancy.
1. Bob clones his `next-best-thing` repo to his local development environment (in your case this would be your Amazon workspace, cloning either through IntelliJ or the command line).
1. Bob makes his modifications on his local copy (either on the default `master` branch or on a branch specific for this change).
1. Bob [pushes his changes](https://help.github.com/en/articles/pushing-to-a-remote) to his fork of the repo.  At this point, Bob can log into GitHub and see his changes.  He is now prepared to create a pull request.
1. Bob [creates a pull request](https://help.github.com/en/articles/creating-a-pull-request-from-a-fork) that is sent _to the original repo_ that Nancy helps to maintain.  Note that this is different than what you will typically do.
1. Nancy reviews Bob's change, providing feedback.  Frequently, Bob will have to [update his pull request](https://stackoverflow.com/questions/9790448/how-to-update-a-pull-request-from-forked-repo) with more commits to address Nancy's concerns.
1. Finally, Nancy is happy with Bob's pull request and [merges](https://help.github.com/en/articles/merging-a-pull-request) it into the authoritative `next-best-thing` repository.  At this point she can decide whether she wants to keep Bob's full commit history, or "squash" it into a single commit.

## Getting Started:
For this lab, you should play the role of Bob in the Overview section above.  Fill out the Interview below, and send me a pull request when you're done!

For each question, please add your response to any other responses already recorded.  Your answer should be formatted similar to the following sample:

Q1: Is this a question?
* _Jeremy_: yes it is

Q2: What is the answer?
* _Jeremy_: Of course, the answer is [42](https://simple.wikipedia.org/wiki/42_(answer)).

## Interview
Hello!  In the rush that is the start of the term, I really haven't had a chance to chat with many of you.  So would you do me the favor of helping me get to know a bit about you by answering the following?  Please avoid one word answers... I want to learn about you!

Q1: So you're finishing up your time in this CSCC program.  Why did you decide to embark on this journey?
* Bobby: I graduated from Miami University as a Software Engineer, but moved into a series of jobs where I worked as either an Infrastructure Engineer or, in the case of my last position, a DevOps Engineer. Unfortunately like all skills, when they aren't being actively used, they stagnate. I was being offered new positions and new fancy "Developer" titles, but at the end of the day, I couldn't help but feel as though I wasn't the true developer I wanted to be, and as each day went on-- my development skills were degrading. I enrolled in this program to help bolster those skills, and to bridge the gap between Academic programming, and Enterprise progamming.

Q2: I _love_ to travel.  Tell me a bit about your favorite travel destination so far.  What's on your travel bucket list?
* Bobby: I'd really love to go to Europe-- preferably somewhere like *Dublin* or *London*
* Jeremy: How about past travel? Any place you've been before (either recently or a long time ago) that you enjoyed? 
* (Edit) Bobby: Well my family lives a bit all over, and have an interesting back-story, so yes I've travelled quite a bit. Growing up, my family's weekend hobby was scuba-diving (whether it was in Lake Michigan where we grew up in Chicago, or the local quarry). On the weekends we'd all go diving and during the summers we were lucky enough to have the opportunity to vacation abroad in countries across the Caribbean (like the ABC islands, Jamaica, Venezuela, Costa Rica, etc.) and the Pacific (Fuji, Hawaii, and Malaysia) for family vacations. Being the youngest of the family, when I left for college, my family sought to their dream of being full-time scuba instructors, so they left Chicago and moved to St. Croix, United States Virgin Islands where they now own and operate their own dive shop [(seen here)](https://www.sweetbottomdive.com/). Because of this, I often fly back and forth to the Virgin Islands, when I'm not busy with work or have military requirements that obligate me to stay back home in Ohio.    

Q3: Name your favorite member of [The Beatles](https://en.wikipedia.org/wiki/The_Beatles), and your favorite Beatles song.  You do know at least one Beatles song, right?  If you are a Beatles fan, feel free to give me your top 5 or so.
* Bobby: Ringo, because I can't help but feel bad for the guy for all the crap the band gave him. But seriously, __all__ members are great; there is no favorite. As for songs, I'd say: _Let It Be_

Q4: Do you have any pets? Species/Name/Details please. [Murray](images/Murray.jpeg?raw) wants to know... (he's not as smart as that picture makes him seem). 
* Bobby: No pets currently, but my folks who live out of the country have our family Wiener dog. His name is Sammy, and by now I'd image the little guy is getting some gray hairs with his brown coat. 

## Submitting Your Work
Once I have merged your pull request into my repo, please submit your repo along with a screenshot of your pull request in Blackboard.

