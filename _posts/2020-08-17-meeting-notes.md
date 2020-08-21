---
title: "August 17, 2020 Meeting Notes"
---
### Carpentries Instructors’ meeting
- Monday, August 17, 2020
- 9:00-10:00 AM

### Present:
Albin, Brooks-Kieffer, Deakyne, Everman, Russell, Trana, Zipper, Koseva (guest)

### Agenda
- Debrief most recent [Software Carpentry workshop, online edition](https://kulibraries.github.io/2020-07-24-ku-online/)

### Materials
This is the first workshop for which we were able to send learners links to the instructors' teaching materials for all of the workshop topics. Yay!
- [Bash Shell by Elizabeth](https://github.com/ereverman/July-August_SWCarpentry_Day1)
- [Version Control with Git by Jamene](https://github.com/jbkieffer/swc-git-script-notes)
- [Plotting and Programming in Python by Matt](https://github.com/mdeakyne/SWC-2020)

### Discussions
Recorded discussion using a live shared document; link upon request if you don't have it. These notes summarize and organize the shared document into topics. Within each topic, discussion points are labeled \+ (positive), &Delta; (change), or ? (question).

**Helping**
- \+ Appreciated dedicated notetaker for Etherpad commands
- \+ Learners having all commands in the Jupyter Lab/Notebook to copy/paste and catch up was also helpful.
- \+ Having notes helped a lot; helping people who got far behind meant re-typing for them what the notetaker was putting in the notes.
- &Delta; Taking notes plus being a helper was hard – tried to do both at the same time for one learner, then passed on notetaking to another person. Designating a notetaker at the beginning and asking learners to check with another helper first will be important for smoother help next time.
- &Delta; This workshop seemed Windows heavy; made it hard for helpers who are Mac users.
- &Delta; Also a lot of need for help versus number of helpers.
- &Delta; Could we set up a concierge for assigning learners to a helper in advance? Based on operating system, number of helpers, number of learners.
- &Delta; As a helper, would be nice if you could show you’re available to help vs. already helping someone. When lots of help was happening, it was hard to know which learners in the main room were waiting, caught up, typing furiously to catch up, or waiting to ask for help.
- &Delta; Turning video on and off could be a way to do that? Or changing background picture, or have a standby screen if busy helping.
- &Delta; Role of helper: in-person, helpers float around the room. Online, helpers need to prep too by installing the software and keeping up; be prepared by budgeting time to get ready for the workshop. Assumption that helpers don’t need to prep is not correct.
- &Delta; It’s easy for helpers to lose track of what is going on; instructor sharing their script in advance would be helpful for helpers to a. prepare and b. catch up if get behind on an unfamiliar topic.
- ? Was concerned about single-screen learners – how would you catch up if you got behind and the instructor’s screen scrolled?
- ? With online workshops, what will we need to give up to keep people on track? Was downloading chat transcripts to see where these moments are.

**Teaching**
- \+ Having a GitHub repository to pull from was helpful, especially during Python 2 - having code that learners could see and then run was called out as helpful in the sticky notes survey. Would be really difficult for a helper to assist a learner working with a blank notebook and the instructor's ever-scrolling screenshare.
- \+ Liked that all teaching materials were in GitHub; instructor recovered well from the git pull going sideways in Python 2.
- \+ People liked the salary data in Python 2; it was approachable.
- &Delta; Perhaps teach a stash at the beginning of Python 2 to stow away the changes they made from Python 1 before pulling more changes from the instructor's repository.
- &Delta; Still have to explain the programming language data when teaching things like what is in the data, what the structure is – relevant for plotting. Bring up research questions for various plots.
- &Delta; Replacing the data set for repeatable teaching means looking up an openly available dataset. Recommended sources mentioned were [Tidy Tuesday Datasets](https://github.com/rfordatascience/tidytuesday) and [Kaggle](https://www.kaggle.com/datasets)
- &Delta; For refining online workshops, thinking about Carpentries' emphasis on typing versus copy/paste; emphasize to learners that typing the commands helps the learning stick, and not to do copy/paste unless they need to. Having the code available can still be helpful for catching up in a crisis.
- ? Possibility of having more than one repository for the Python materials from Python 1 to Python 2? Now that materials are built, probably one repository for next time, and learners may not even have to pull on the second week of the programming language.

**Anaconda**
- &Delta; Launching Jupyter Lab/Notebook for the first time needed a huge pause; needed to pause again the second week of Python, but checked in more frequently.
- &Delta; This is important for the Python section; installing Anaconda is not trivial; need a check right off the bat to confirm installation.
- &Delta; Is this an area where some more familiarity with what happens on Windows vs. Mac would be helpful for instructors and helpers? Anaconda doesn't set the path environment variable on Windows by default, so some of our Windows users needed to launch the additional Anaconda Prompt to open Jupyter Notebook/Lab, or get help from a Windows helper who knew how to get around this problem.
- &Delta; Differences between Git Bash and Anaconda Prompt caused Windows users a lot of confusion.
- &Delta; Even helpers had trouble with Anaconda on Windows this time. Having Anaconda install for all users on Windows causes problems; messes up the path environment variable for all user accounts on the computer. Even on re-install, the path command in Git Bash didn’t work for Casey unless he manually set the path variable.
- &Delta; Teaching how to close Jupyter Lab/Notebook is important, since learners can be overwhelmed with new information and miss how to do this the first time.

**Zoom**
- \+ Escalating problems from helper to room host to instructor seemed to work okay; hard for instructor to leave the main room – good to do this during a break.
- \+ Having helpers put OS in Zoom name was helpful.
- &Delta; Learners should also put their OS in their Zoom name.
- &Delta; Learned that helpers need extra steps online to assess the need for help:
  - Are you already being helped?
  - What kind of computer are you using?
  - These are things that are immediately visible in an in-person workshop.
- &Delta; Create a strategy for breakout rooms because of Zoom’s limitations with who can create breakout rooms (only the Host). Instructor and room host should stay in the main room if at all possible.

**Workshop Overall**
- \+ Workshop retention was good, especially compared to Carpentries conversations about online workshops overall.
- &Delta; Distinctions between people who were there the week before vs. people who weren’t and what they need to do to be ready for the teaching part.
- &Delta; Visiting with learners during beginning is not possible in online environment.
  - Idea for staged emails before each lesson – 3 gradually more specific emails with more and more information.
  - No way to get around people who don’t read the emails.
  - Budget in an extra 15 minutes for checks to get everyone on the same page – takes 10 min from instruction, but prevents car crashes at the beginning.
  - Split people out into breakout rooms to do this? Based on OS as one way.
  - Easier to get learners to share screen in a smaller breakout room.
- &Delta; Helpers knowing how to pause the instructor is important; a scheduled major check at the beginning could also address this. Can be intimidating to unmute and pause the workshop. Be upfront with helpers that they should unmute and pause the workshop.
- &Delta; Important to remember that most of the people who were lost were lost before the instructor started typing.
- &Delta; Giving time during a break or at the end to ask their specific questions during the workshop. This is something that happens regularly in an in-person workshop (these are the fun conversations).
- &Delta; Idea to conclude each day with a Git repo for next time; to catch up people who weren’t able to come the week before.
- ? Suggestion of 2 lessons per week from a learner - would that help with re-using data? People might be less likely to forget what they were doing  


Notes by JBK
