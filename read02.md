# Where the world builds software 
## Millions of developers and companies build, ship, and maintain their software on GitHub—the largest and most advanced development platform in the world.
# Version Control
Version control, also known as source control, is the practice of tracking and managing changes to software code. Version control systems are software tools that help software teams manage changes to source code over time.
# Centralized Version Control
Centralized version control systems are based on the idea that there is a single “central” copy of your project somewhere (probably on a server), and programmers will “commit” their changes to this central copy. “Committing” a change simply means recording the change in the central system
What Is a Distributed Version Control System (DVCS)?
A distributed version control system (DVCS) is a type of version control where the complete codebase — including its full version history — is mirrored on every developer's computer. It's abbreviated DVCS.
![changes](https://marvel-b1-cdn.bc0a.com/f00000000075552/www.perforce.com/sites/default/files/image/2018-07/image-blog-what-is-dvcs.jpg)

## Changes to files are tracked between computers
For example, my workstation and yours. In the beginning, this required specific coordination strategies to maintain consistency in projects, so all the developers could keep track of what was happening to files at any given time.
What Is a Distributed Version Control System (DVCS)?
A distributed version control system (DVCS) is a type of version control where the complete codebase — including its full version history — is mirrored on every developer's computer. It's abbreviated DVCS.
![data analysis](https://blog.udemy.com/wp-content/uploads/2015/08/image066.png)

## So, what is Git?
1. **Snapshots**

Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.

2. **Local Operations**

Git mostly relies on local operations because most necessary information can be found in local resources. This allows for process expediency because a project’s history resides on the local disk, eliminating the need to fetch history information from the server, and allowing one to continue work on a project even when not online or on a VPN.

3. **Tracking Changes**

Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

4. **Loss of Data**
Git is set up to greatly minimize the possibility of irreversible damage to files, such as accidentally lost data. Git makes it extremely difficult for a snapshot of your file that is committed to be lost.

5. **States**
Files in Git can reside in three main states: committed, modified and staged.

6. **Committed**
Data is securely stored in a local database

7. **Modified**
File has been changed but not committed to the database

**The History of Git The Road to Domination in Software Version Control**
*In 2005, Linus Torvalds urgently needed a new version control system to maintain the development of the Linux Kernel. So he went offline for a week, wrote a revolutionary new system from scratch, and called it Git. Fifteen years later, the platform is the undisputed leader in a crowded field.
Worldwide, huge numbers of start-ups, collectives and multinationals, including Google and Microsoft, use Git to maintain the source code of their software projects. Some host their own Git projects, others use Git via commercial hosting companies such as GitHub (founded in 2007), Bitbucket (founded in 2010) and GitLab (founded in 2011). The largest of these, GitHub, has 40 million registered developers and was acquired by Microsoft for a whopping $7.5 billion in 2018.*
![changesS](https://blog.udemy.com/wp-content/uploads/2015/08/image006.png)

What are developers using for source control?

|           2018         |          2015          |
| ---------------------- | ---------------------- |
| Git: 88.4%             | Git: 69.3%             |
| Subversion: 16.6%      | Subversion: 36.9%      |
| Team Foundation: 11.3% | Team Foundation: 12.2% |
| Mercurial: 3.7%        | Mercurial: 7.9%        |
|                        | CVS: 4.2%              |
|                        | Perforce: 3.3%         |

| 74,298 responses       | 16,694 responses       |

Source: **Stack Overflow Developer Survey 2018/2015**

Local Repository Structure
The local Git repository has three components:

**Working Directory:** The actual files reside here.
Index: The area used for staging
Head: Points to the most recent commit*
Ignoring Files
Usually, untracked files consist of uncommitted files recently added to a project or compiled binaries with extensions such as .exe and .obj. Compiled binaries can make it difficult to clearly monitor your repository. Git allows users to avoid this situation by ignoring certain files by sending them to a special file with the name .gitignore.

**Note:** It’s always wise to check your repository before committing anything, to avoid accidentally committing certain files.

*Files that all developers should disregard go into a .gitignore file.
Every line within a gitignore file indicates a pattern.
Additional information regarding gitignore files can be found.*
Renaming/Removing Remotes
Rename

## To rename a remote’s short name, use the git remote rename command.

Example:

$ git remote rename js jane

$ git remote

origin

jane
*In the example above, we can see that the remote’s short name has been changed from js to Jane. The command git remote lists our existing remotes, which jane is now one of. The rename action also alters names of remote branches: js/master would change to jane/master.

Remove

To remove a remote for whatever reason (e.g., a contributor has left the team, the server has moved), simply use the git remote rm command:

Example:

$ git remote rm jane

$ git remote

## origin
NOTE: Reminder: “origin” is simply the default remote name when you use the git clone command.

my view link https://yazan994.github.io/reading-notes/read02