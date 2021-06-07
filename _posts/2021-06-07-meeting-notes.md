---
title: "June 7, 2021 Meeting Notes"
---
### Carpentries Instructors’ meeting
- Monday, June 7, 2021
- 9:00-10:00 AM

### Present:
Brooks-Kieffer, de Mello, Deakyne, Everman, Kindred, Russell

### Agenda
- Brief Introduction to Docker (Matt)
- Discuss possible workshop topics and timing for the remainder of 2021
- Discuss workshop formats for the remainder of 2021: in-person, online, or a mix

### Discussions

**Brief Introduction to Docker**

Despite zero advance notice, Matt was willing to do a brief demonstration and introduction to Docker containers for the group. With some notice for the next meeting, he can prepare a more Carpentries-specific demo, maybe with some hands-on. Thanks, Matt!

Docker helps set up and contain all the environments and packages needed for a specific project. Matt demonstrated a Docker container he is using during KU's transition from Blackboard to Canvas. He opens a Dockerfile, pulls in an existing Python image maintained by Docker, then starts adding an Oracle client and Python packages needed for the project. He is then able to open a new root user shell in this environment. Inside this environment, there's no access to files on the local computer, so Matt showed a workaround that involves launching a Jupyter Lab instance in the environment that can then interact with the local computer. He also uses Jupyter Lab and GitLab to share his containers and code with colleagues, so the work doesn't have to happen only on his computer.

Advantages include not having to run local installations of packages, avoiding dependency hell, and sharing project functionality across all operating systems. He is using [VS Code](https://code.visualstudio.com/) as his IDE; he endorses because it can make some of the harder parts of Docker easier and more behind-the-scenes.

There is a [Carpentries Incubator lesson for Docker](https://carpentries-incubator.github.io/docker-introduction/); the group briefly discussed the idea of a code + container workshop series. Although it might not be the best fit for new graduate students, a series like Intro Python (or R), followed by Docker, followed by a lesson to combine the two might be a good fit for researchers. Another possibility might be a two day equivalent workshop assembled from shell + intro language + container lessons.

There was lots of discussion around this intro, with many folks having experience with environment managers like conda and some having experience with Singularity (containers for HPC). It seems like the group will be really interested in some hands-on time with Docker in the future. In the meantime, Matt shared a list of 3 installations for getting started:

1. [Docker](https://www.docker.com/products/docker-desktop)
2. [MS VS Code](https://code.visualstudio.com/)
3. [Remote Development extension pack](https://aka.ms/vscode-remote/download/extension)

**Potential Workshop Topics and Timing**

Besides the idea mentioned above about a code + container series, folks contributed ideas for workshops during the rest of 2021:

- Intro to R (requested by KBS)
- DC-Geospatial (discussed during the [May 3](https://kulibraries.github.io/carpentries-instructors/2021/05/03/meeting-notes.html) meeting)
- Something in-person (see next topic below)
- Brainstorm possible workshop topics via email and offer the list as a survey to graduate student groups, e.g. SACNAS, EEB GSO, MB GSO, etc. to see what students are interested in. Jamene will start an email thread for this brainstorm.

Folks seemed to think that full workshops as well as single topics are possibilities for late summer and fall.

**Workshop Formats**

Folks are interested in all possible formats: fully in-person, fully-online, and hybrid. A discussion ensued to define various interpretations of "hybrid":

- Online instructor + in-person learners
- Mix of online and in-person learners
  - In semester-long classes this has proven difficult, but might be possible over a two-day workshop if there were designated in-person and online helpers to pull the instructor's attention to where it's needed.
- Multiple sites participating in the same workshop, e.g.: two connected locations for in-person learners and instructors sharing the sessions with each other.
  - The Great Plains Network Carpentries instructors have done this before - Jamene can ask for experiences at the next meeting of this group.
  - Classroom locations for this kind of hybrid at KU include Pharmacy classrooms, possibly Price Computing Center Auditorium, and possibly Libraries classrooms

There was agreement that any version of a hybrid workshop is going to be more personnel-intensive than either fully in-person or fully online.

There was also agreement that in-person incentives (coffee, snacks) will be important for helping people feel comfortable coming back to an in-person environment. This led to an extensive discussion of cookies, brownies, flourless chocolate torte, and brigadeiro.


Notes by JBK
