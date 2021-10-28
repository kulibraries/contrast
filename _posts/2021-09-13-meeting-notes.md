---
title: "September 13, 2021 Meeting Notes"
---
### Carpentries Instructors’ meeting
- Monday, September 13, 2021
- 9:00-10:00 AM

### Present:
Albin, Brooks-Kieffer, Everman, Flynn, Koseva, Russell, Thomas, Trana, Zipper

### Agenda
- Updates on [modular Software Carpentry workshop](https://lib.ku.edu/software-carpentry) 9/24-12/03
- Debrief [Data Carpentry Geospatial](https://kulibraries.github.io/2021-08-04-ku-dc-online/)
- Tricky Helper Topic: Cloud storage defaults that cause trouble (Samantha)
- Carpentries lesson status indicators
- Other Topics

### Discussions

**Updates on modular Software Carpentry workshop**

These one-topic workshops will take place one Friday per month. Schedule is:

- Python: September 24 (Matt) - full day
- Bash Shell: October 1 (Rob and Casey) - half day
- Git: November 5 (Pietro and Tami) - half day
- R: December 3 (Thane and Matt) - full day

We will charge a $10 refundable deposit for each registration. Eventbrite has changed its refund policies since we last charged a deposit; initially it was not clear that registrants would be able to receive a full refund. It seems to be working for now, but we will need to stay aware of the policies for future workshops.

**Debrief Data Carpentry Geospatial**

[Data Carpentry Geospatial](https://kulibraries.github.io/2021-08-04-ku-dc-online/) happened August 4-5 with Samantha and Sam. Attendance was consistent at around 15 people (capped at 20). The topics didn’t feel rushed. Helpers didn't have as much troubleshooting to do because it was an advanced topic and maybe people were already prepared on the basics. It was helpful to have already practiced the Docker installation for Mac users; this was needed to get one Mac user access to the necessary R packages. Most learners and instructors were Windows-based. Etherpad was helpful; a helper notetaker kept the Etherpad content up to date, and instructors used it to post exercises and challenges. Instructors did a good job of incorporating these smoothly into the lessons. One learner encountered challenging software problems caused by using cloud storage defaults (thus the next topic).

**Troublesome Cloud Storage Defaults**

During the recent Data Carpentry Geospatial workshop, one learner encountered software installation issues caused by having cloud storage defaults set on their computer (in this case, OneDrive was the location). In R, the libraries were downloaded to OneDrive, but attempting to install from a local library path. This took 3 helpers a long time to solve. One possible solution is to specify the library path during the install, but that wasn’t helping this case. The learner had downloaded the RStudio files to OneDrive so they didn’t have to keep downloading and installing the files to different computers – this may have been one of the root causes for this problem.

Possible solutions:
- Rtools global options, specify download paths
- Change the R profile to specify download paths
- Examine the $PATH - if an older install is still in the $PATH, the computer will never find the newer install further down the $PATH

**Carpentries Lesson Status Indicators**

Most Carpentries lessons now have a status indicator: pre-alpha, alpha, beta, and stable. Pre-alpha is the first lesson status, when a lesson is proposed and in development but has not been taught. Alpha has been taught by its developers and is looking for feedback from other instructors. Beta has been taught by a variety of instructors and undergoing further refinement. Stable is released as a part of the main curricula. Any stage of lesson can be taught but may not be fully complete with enough material or a perfect match up between the learning outcomes and what is covered. When teaching a lesson in a development stage, it's very helpful to provide feedback to the lesson developers.

**Other Topics**

Boryana attended a 3 day online workshop from UC Davis; while the first day of the workshop was something of a mess in terms of paths, permissions, and other logistics, the instructor did a really good job of normalizing turning on cameras at the beginning of a lesson and before a break, asking people to introduce themselves and ask questions out loud, and other community-building. Boryana also liked that learners were put into smaller groups in breakout rooms to work on exercises together.

Casey has struggled in the past to apply data science work to his regular duties. Recently was asked by a client for a report on network traffic and firewall blockages; client had not been saving the monthly reports they already received. Casey acquired the archived network traffic data from logs and has gotten it cleaned up and ready for analysis. The only way to get the archived files into .csv was through a web interface – he collected lots of files manually.  Suggestions for future development included Selenium for Python – Selenium is a package that mimics a web browser so you can script all kinds of web browser behaviors like clicking buttons and filling in fields. Other suggestions included bash scripting and curl, depending on the URL path structure.

Notes by a mystery contributor, posted by JBK
