---
title: "July 12, 2021 Meeting Notes"
---
### Carpentries Instructors’ meeting
- Monday, July 12, 2021
- 9:00-10:00 AM

### Present:
Brooks-Kieffer, Dwyer, Everman, Kindred, Koseva, Russell, Trana, Wilhelm

### Agenda
- Updates on workshop topics and timing for the remainder of 2021
- Update on idea for a two-site workshop
- Check in on instructor training and checkout
- `git detached HEAD` demo (Jamene)

### Discussions

**Updates on workshop topics and timing**

[Data Carpentry Geospatial](https://datacarpentry.org/lessons/#geospatial-curriculum) workshop planning in progress for the first week of August. Registrants will need some R experience. This workshop will be online to accomodate learners and helpers from various institutions. The group talked previously about leading with an Intro R workshop, but this won't be possible this time.

At the [June](https://kulibraries.github.io/carpentries-instructors/2021/06/07/meeting-notes.html) meeting the group showed a lot of interest in Docker. We could offer a Docker workshop before the end of the year using [lesson material](https://carpentries-incubator.github.io/docker-introduction/) in The Carpentries Incubator. Lots of details to work out to make this happen.

Other ideas for upcoming workshops: Most previous workshops have had waitlists without a lot of drop off, especially when the lesson days were closer together. There is interest in Intro to R from Kansas Biological Survey. If there are lots of other opportunities to get experience with a particular topic, offer workshops on topics that are less accessible. May be time to do a Python workshop.

**Two-site workshop idea**

The proposed format is for two in-person classrooms that are at different universities connected by Zoom. Instructors could be in only one location or in both; helpers would be in both locations. This is a way of approaching the use case of one institution gaining experience in hosting and instructing Carpentries workshops by partnering with an institution with more experience. The format may be useful for institutions participating in AIMS and for folks working with smaller institutions. Several instructors are interested in pursuing this further.

KU has several rooms where this is possible, notably in Pharmacy, which teaches classes co-located in Lawrence and Wichita. It's important to remember the student perspective. This can be a challenging environment to learn in, and it can be difficult to connect with online learners, helpers, and moderators.

Perspectives from other Carpentries instructors in the region who have tried this include:

- Glitches at one site affect the other site, too
- Test the rooms thoroughly to understand the equipment and how to get help
- Practice for possible problems such as network outages
- Have learners log into Zoom to show their video at least occasionally; be prepared for audio  feedback if learners forget to mute themselves

**Check In on Instructor Training and Checkout**

Advice on the lesson contribution checkout task: can contribute to any of the lessons. This is an exercise to help get familiar with the process of contributing and using the lesson maintenance tools. Contributions can take the form of a pull request offering a fix for an identified issue or an issue describing the problem and its fix. Lesson maintainers keep a list of identified problems that can be used to complete this checkout task: [https://carpentries.org/help-wanted-issues/](https://carpentries.org/help-wanted-issues/)

Teaching Demo advice: you don’t know the specific episode you will teach from, but you specify which lesson/topic. The organizer will pick an episode for you. Usually not the first or last lessons; the episode will have live coding components. Recording yourself can be useful to gauge speed and delivery as well as to figure out about how much of an episode you can get through in 5 minutes (spoiler: not much).

Getting an extention for completing checkout tasks is straightforward, but it's important to request it before your deadline. Ask Jamene for help if needed.

**`git detached HEAD` demo**

As part of the Tricky Helper Topics professional development series we discussed in [March](https://kulibraries.github.io/carpentries-instructors/2021/03/01/meeting-notes.html), Jamene presented on the topic of `git detached HEAD` using a [GitHub repository](https://github.com/jbkieffer/holiday-fun) she created to teach fork/branch/pull request.

To follow along, open a command line environment and clone the repository:

`git clone https://github.com/jbkieffer/holiday-fun.git`

Inside the directory, display the commit history. This repo has 4 commits:

`cd holiday-fun`

`git log --oneline`

The Carpentries Git lesson teaches checking out a specific file at a specific commit or point in time. Instead of doing that, we checkout the entire repository at a specific commit (here, the oldest commit in the log); this results in detached HEAD state:

`git checkout 71ad081`

We can look around at the state of the repository in this commit, but we shouldn't make any changes that we want to happen in this branch of the repository. Basically, we've gone back in time, so we need to be very careful.

 If we want to use this state of the repository as a baseline for a related project, we can create a branch while we're back in time. In this case, we use the holiday party README as a starting point for planning a summer pool party in a separate branch:

 `git checkout -b pool`

 Now we can make more changes and commit them to the `pool` branch without affecting the `master` branch where the holiday party planning is happening. To switch back to the `master` branch, we use:

 `git checkout master`

 This is also the command that will fix detached HEAD state if you wind up here by accident.

 Full documentation about the `git checkout` command is available at [https://git-scm.com/docs/git-checkout](https://git-scm.com/docs/git-checkout).


Notes by ERE, posted by JBK
