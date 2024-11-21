- **Git** for **software version control**
- **Maven** to **mange software builds**
- Use **IntelliJ Debugger**
- Software package **Bagel** (Basic Academic Graphical Engine)
- Importance of contributing to **Open Source Software** (OSS) projects  
# Version control with Git
Software version control:
- Systematic way to manage concurrent versions of software (documents, source code, data, etc.)
- As an individual: keep software saved
- In a team: allows developers to write and test code locally before including that to code base
## The git model
- **Repository**: collection of files to be stored by the version control system + metadata
- **Remote repository**: a repository maintained in a remote server (GitHub, Bitbucket, GitLab)
- **Local repository**: a repository maintained in the local directory -  in `.git`sub directory.
- **Index (staging area)**: a conceptual place for staging the changes - in `.git` sub directory.
- **Working directory**: the local directory  where files are kept and modified
![center|](attachments/Screenshot%202024-08-06%20at%2014.30.17.png)
## The git model - branching
![Screenshot 2024-08-06 at 23.27.54](attachments/Screenshot%202024-08-06%20at%2023.27.54.png)
## The git model - merging
![Screenshot 2024-08-06 at 23.28.14](attachments/Screenshot%202024-08-06%20at%2023.28.14.png)
## Using git
Subject remote repo: https://swen20003.eng.unimelb.edu.au/

1. Copy the `[clone URL]` (clone with HTTPS) of the project on GitLab
2. Make a local copy of the repo:
	- `cd` to where you want to store the local copy
	- enter `git clone [clone URL]`
3. Stage files:
	- copy files into working directory
	- `cd` to the working directory
	- to stage all files: `git add .`
	- to stage specific files: `git add [file name]`
4. Update local repo:
	- `git commit -m "[message]"`
	- `[message]` is a meaningful message used to describe changes
5. Update the remote repo:
	- `git push`
	- add changes to the master branch of the remote repo: `git push -u origin master`

NOTE: working directory contains the `.git` file. List hidden files using `ls -a`.
## Other useful git commands
![Screenshot 2024-08-07 at 00.19.38](attachments/Screenshot%202024-08-07%20at%2000.19.38.png)
# Build management with Maven
- Software build management tool
- Simplifies the process of building software by automatically importing libraries and dependencies from external repositories
- In Maven, the project structure and contents are declared in an xml file, Project Object Model (POM) - pom.xml

# Using the IntelliJ Debugger
![Screenshot 2024-08-08 at 22.50.34](attachments/Screenshot%202024-08-08%20at%2022.50.34.png)
# Bagel
**Bagel** (Basic Academic Graphical Engine) is a custom graphics package for Java
# Open Source Software (OSS) projects
https://www.firsttimersonly.com/
https://roshanjossey.github.io/first-contributions/
https://www.codetriage.com/
https://up-for-grabs.net/





