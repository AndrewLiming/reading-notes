# Read: 03 - Revisions and the Cloud

these are my notes for todays reading assignment

Version Control is a system that lets you go back to different versions of your file. Using VCS, you can track mods and who modded it and fix mistakes. Local VCS is a database on your hard drive. Centralized VCS is for collaboration within a developer team. It uses a single server that can be accessed by various clients. It streamlines the process, allowing every to collaborate. Distributed VCS or DVCS allows clients to create mirrored repositories which helps safeguard against a single server going down.

Git is a DVCS. It creates snapshots of the file and stores a reference to the changes using the commit action. Git mostly relies on local operations as most of the information is found in local resources. This streamlines the process as, since the data is stored on a local drive, theres no need to access the history so you can even work offline. Every change made to files or directories is tracked by Git/ It will always detect corrupted files and loss of information. Its set up to minimize damage to files or lost data. Files can reside in commited, modified or staged states. commited means the information is stored in your local database, modified means the file has been changed but not yet commited and staged means the files changed version has been flagged to be commited in the next snapshot.

History of Git: Git traces back to a software project called Linux kernel. it began as a DVCS called Bitkeeper in 02. In 05, there was tension between linux kernel users and the bitkeeper company which caused the DCVS to stop being free. Linus Torvalds created Git to serve as a Bitkeeper replacement but faster. Git allows for non-linear development via multiple branches, can support larger projects, prevents file corruption and is easy to use. In the past 15 years, it has become one of the most popular VCS' in the world.

Git can be installed as a package, installed through another installer, or you can download and compile the source code.
The easiest method to install Git on a Mac is running it from the terminal. You can also install it straight from their site or through Github for both Mac and Windows. You can install Git for Linux through your package management tool.

Graphical Clients. Git uses Graphical User Interface (GUI) tools. You can also use third party tools. 

Initial Customization: after youve installed Git, you should customize it. You should configure it using git config and set your email address and user name using `git config --global user.name "Jane Smith"` and `git config --global user.email "example@email.com"`. using the global option sets git to apply it to everything in the system. you can change it to be project specific by using that code without the --global.

You should set your defult text editor if you dont want to use Git's default one. you'll want to type in  `$ git confi --global core.editor "fill in blank"` to pick your specific text editor.

Next you'll want to type in `git config --list` to check your settings.

To get help, you'll want to type in one of three possible prompts, `git help command`, `git command --help`. or `man git-command`.

To set up a Git Repository, you'll want to switch to the target directory using something like "`$ cd test (cd = change directory)`" and then use the git init command "`$git init`". Youve now vreated a new subdirectory named .git that has your repository files. To start tracking, type the following "`$ git add *.c`", "`$git add LICENSE`", `git commit -m "your message"`.

To clone your files to the terminal, type "`$ git clone "your files address"`. To clone a repository into a directory with another name of your choosing, use the following command format "`$ git clone "desired address" mydirectory`". That will make a copy of the target repository in a directory titled "mydirectory".

Local Repository Structure has three components 
- Working Directory: where the files reside
- Index: the area used for staging
- Head: Points to the most recent commit

All files in a working copy of a project file are either tracked or untracked. Tracked files can be modified, unmodified, or staged. Untracked files werent in the last snapshot and dont currently reside in the staging area. After you clone a repository, files have tracked status but are unmodified because they have been checked out but not edited.

Life cycle of file status. after you edit the file, git flags it as modified because of changes made after the previous commit. you stage the modified file. then you commit staged changes.

Tracking and staging a new file, for a single file you'll use "`git add filename`", for all files, you'll use "`$ git add *`". After that, files are now tracked and staged for commiting.
To commit a single file, you'd use the command "`$ git commit -m "(description of changes)`".
To commit all changes, you'd use command "`$ git commit -a`".

[table of contents](https://andrewliming.github.io/reading-notes/)