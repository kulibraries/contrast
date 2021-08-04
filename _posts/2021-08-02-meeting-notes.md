---
title: "August 2, 2021 Meeting Notes"
---
### Carpentries Instructors’ meeting
- Monday, August 22, 2021
- 9:00-10:00 AM

### Present:
Albin, Brooks-Kieffer, de Mello, Deakyne, Dwyer, Everman, Russell, Trana, Thomas

### Agenda
- Brief update about [Data Carpentry Geospatial](https://kulibraries.github.io/2021-08-04-ku-dc-online/)
- Tricky Helper Topic: Add a program to the user $PATH (Casey)
- Ideas, staffing, and format for Fall Carpentries workshops

### Discussions

**Data Carpentry Geospatial**

[Data Carpentry Geospatial](https://kulibraries.github.io/2021-08-04-ku-dc-online/) workshop is happening Wednesday and Thursday, August 4-5, 2021. This is the traditional two-day format, although the workshop will take place online. Learners are expected to have some existing R experience. Software installation for this workshop was not straightforward during testing; the Docker option offers a slightly easier way to access the necessary R packages, especially on a Mac.

**Installing a program on the user $PATH**

The $PATH is an always-on environment variable that the computer uses to look up where to find the executable for a program name that a user types in. If there’s no $PATH entry for a program, the computer can’t execute the program even though it’s installed. The same thing happens if there’s an existing program with a different location.

Python is kind of notorious for this happening. It occurs at workshops when Windows users install Anaconda for the Python lesson. Anaconda installs its own Windows command prompt and Windows PowerShell prompt on Windows, so users can interact with conda via one of those terminals. Windows-based learners who are told to open Anaconda using the GitBash command line will get an error because Anaconda hasn’t written itself a $PATH entry in GitBash.

Casey’s demo uses GitBash, so a Linux environment. Windows has its own $PATH, and so does macOS.

To see what’s in the $PATH variable, at the command prompt (on nearly all OSs; case matters):

`echo $PATH`

Casey demonstrates adding the Desktop directory as a location for the computer to look for an executable: (this syntax adds this line to the top of the path, followed by the rest of the PATH)

`export PATH=/c/Users/name/Desktop:$PATH`

This method is session-dependent – it will go away when the session ends. There are lots of ways to make these permanent; these vary across systems. Can make it permanent for bash only, for zsh only, for Windows only, or global for all users. There are lots of options.

`ls /etc/profile.d`

On Linux systems, this is the location for aliases, profiles, and other stuff that the shell executes when it opens, as long as the file is a shell script (.sh). You have to run GitBash as administrator to write a file to this location.

`nano /etc/profile.d/desktop_path.sh`

`Export PATH=$PATH:/c/Users/name/Desktop`

Save and close the shell script.

When you check the contents of the $PATH after doing this, the new entry may not be where you expected it to be; doing this isn’t exactly like doing the session-specific edit above.

It’s also important to remember that the computer will execute the $PATH from top to bottom in order. If you have two entries for a program, the computer will only ever execute the one that’s first. This can make for frustrating troubleshooting if you have an installed program that the computer won’t run.

Matt brings up .bashrc and .zshrc, which sets preferences specific to one shell. This is the correct technique for a non-administrator on an HPC or other shared resource, where the user doesn’t have access to administrative privileges. The profile technique that Casey showed will correct the $PATH system-wide, which is more appropriate for a single user who’s the primary user of their machine.

**Ideas, staffing, and format for Fall Carpentries workshops**

People are interested in Carpentries workshops around campus. There is a lot of interest for intro R, and we haven’t offered Python for a year. In addition, AIMS affiliates may need or want Git and GitHub.  

Jamene floated the idea of a modular workshop. Offer the elements of Software Carpentry separately (Bash, Git, Python, and R) as standalone events and allow people to register for as many or as few as they find relevant. Scheduling is maybe easier because this method removes dependency between topics and places some responsibility on learners to know their skillset.

There was interest in adding accountability measures by bringing back the workshop deposit or holding the events in person. These would be good opportunities for new instructors to teach their first workshop. The languages are part 1 and 2 – some interest in making the language a full-day event so there’s no concern with getting people back for part 2 or making sure that part 2 attendees have had part 1. There was also discussion of ways to record or offer asynchronously the software setup instructions and some ways to test an installation. As an example, the KU HPC folks have put up some [instructions about basic operations](https://crc.ku.edu/hpc/how-to).

Spacing: one a month? Have some type of connection between the topics? Give context for the skills to be able to learn other skills later.

Idea to start with a humanities dataset – have the dataset that the series starts with be the “connectivity” or story for the series – this thread began as a question about whether humanists would be likely to sign up for the Bash topic. Kaylen’s take: the workshop needs to be task-based in a way that’s relevant while also teaching the tool; [HathiTrust Research Center workshops](https://www.hathitrust.org/htrc_workshops) are good at this.

More to come on this topic, likely via email.

Notes by a mystery contributor, posted by JBK
