---
title: "January 10, 2022 Meeting Notes"
---
### Carpentries Instructors’ meeting
- Monday, January 10, 2022
- 9:00-10:00 AM

### Present:
Albin, Brooks-Kieffer, Burgin, de Mello, Deakyne, Dwyer, Everman, Kindred, Koseva, Loecke, Russell, Thomas, Trana

### Agenda
- Introductions for new folks and the new year
- Check in on instructor training and checkout tasks
- Planning for Data Carpentry Genomics
- Tricky Helper Topic: zsh vs bash on MacOS
- Open discussion time

### Discussions

**Instructor training and checkout tasks**

Insights from folks who have completed one or both of these:

- It's possible to over-prepare for the teaching demonstration
- Download any datasets or intermediate files you may need for the lesson you're teaching in advance of your demo
- Contributions to lesson materials don't need to be large or accepted. They're meant to demonstrate that you can interact with the lessons and how they're maintained.
- Lesson contribution can be a pull request OR an issue
- Training isn't difficult or arduous, but it's easy to put off, so try to get it done
- Can request an extension from The Carpentries if you need one
- Schedule the teaching demo early because slots are limited to a certain number of participants and they fill quickly

**Data Carpentry Genomics**

Boryana and Elizabeth leading the workshop, aiming for 3 full days, possibly the week of February 14 (post-meeting update: will be February 15-17, 9-4 all days). Pietro and Samantha offered to help; suggestions for additional helpers included helpers from previous DC-G. Registration capped at 20, so aim for 4-5 helpers available at any one time. The helper signup sheet will include topics for each half day so helpers can self-select their date/time slots. This workshop uses AWS deployed by The Carpentries; as a result, software installation is really easy. Learners from CMH will need some help from IT to be able to access a remote connection in the shell.

**Tricky helper topic: zsh vs. bash on MacOS**

Boryana talked us through possible issues learners will encounter in Data Carpentry Genomics as a result of changes to newer versions of MacOS that make zsh the default shell instead of bash. The primary issue is a bug that prevents secure file transfer between a remote and a local computer on zsh. There is a line of code that can fix this; learners would need to paste it into their zprofile. An easy solution for DC-G will be to have every learner type the command to use the bash shell. On Windows (Git Bash) and older Macs the command won't hurt anything, and could save some confusion and troubleshooting for newer Mac users.

**Open discussion**

Kaylen and Jamene are working on a Spring workshop about OCR (Optical Character Recognition) using a command-line tool called [Tesseract](https://tesseract-ocr.github.io/tessdoc/Home.html). The lesson would include instruction on the Bash shell and then Tesseract. Tesseract requires administrative permissions to install; Kaylen is looking into ways to get around this. Remote computing may be a way to solve this problem. Kaylen and Jamene may talk more to Casey and Boryana for advice.

Notes by ERE, posted by JBK
