## Ch03_Working with Git Locally

<!-- toc orderedList:0 depthFrom:1 depthTo:6 -->

- [Ch03_Working with Git Locally](#ch03_working-with-git-locally)
	- [12. Starting Fresh](#12-starting-fresh)
	- [13. Starting with an Existing Project](#13-starting-with-an-existing-project)
	- [14. Starting Commands](#14-starting-commands)
		- [Git Starting Commands](#git-starting-commands)
			- [Lecture Command Listing - Fresh Start](#lecture-command-listing-fresh-start)
			- [Lecture Command Listing - Start with Existing Project](#lecture-command-listing-start-with-existing-project)
			- [Command Reference](#command-reference)
	- [15. The First Commit](#15-the-first-commit)
	- [16. First Commit Commands](#16-first-commit-commands)
		- [Git First Commit Commands](#git-first-commit-commands)
			- [Lecture Command Listing](#lecture-command-listing)
			- [Command Reference](#command-reference-1)
	- [17. Working Locally, Part 1](#17-working-locally-part-1)
	- [18. Working Locally, Part 2](#18-working-locally-part-2)
	- [19. Working Locally Commands](#19-working-locally-commands)
		- [Git Working Locally Commands](#git-working-locally-commands)
			- [Lecture Command Listing - Working Locally, Part One](#lecture-command-listing-working-locally-part-one)
			- [Lecture Command Listing - Working Locally, Part Two](#lecture-command-listing-working-locally-part-two)
			- [Command Reference](#command-reference-2)
	- [20. Gitting Historical](#20-gitting-historical)
	- [21. Removing Files](#21-removing-files)
	- [22. Moving Files](#22-moving-files)
	- [23. Ignoring Files](#23-ignoring-files)
	- [24. History and File Management Commands](#24-history-and-file-management-commands)
		- [Git History / File Management Commands](#git-history-file-management-commands)
			- [Lecture Command Listing -- History](#lecture-command-listing-history)
			- [Lecture Command Listing -- Removing Files](#lecture-command-listing-removing-files)
			- [Lecture Command Listing -- Moving Files](#lecture-command-listing-moving-files)
			- [Lecture Command Listing -- Ignoring Files](#lecture-command-listing-ignoring-files)
			- [Command Reference](#command-reference-3)

<!-- tocstop -->

### 12. Starting Fresh  

### 13. Starting with an Existing Project  
  * Initial website files (initializr. com)    
    * http://www.initializr.com/

### 14. Starting Commands  
---
#### Git Starting Commands

##### Lecture Command Listing - Fresh Start

```
pwd
cd projects/
git init git-demo
```

##### Lecture Command Listing - Start with Existing Project

```
pwd
cd projects/
cd website/
ls
git init
```

##### Command Reference

Present Workding Directory

```
pwd
```

Change Directory

```
cd
folder-name
```

Git initialization

```
git init [project-name]
```

project-name_parameter is optional. If not supplied, Git will initialize the current directory.

---

### 15. The First Commit  
  * Git Workflow Wd  
  * Git Workflow Stage  
  * Git Workflow Commit  

### 16. First Commit Commands  
---
#### Git First Commit Commands

##### Lecture Command Listing

```
pwd
ls
mate README.md
ls
git status
git add README.md
git status
git commit -m "Initial commit"
clear
git status
```

##### Command Reference

List

```
ls
```

Lists files and folders in current directory. Without parameters, will list non-hidden folders and files.

Git Status

```
git status
```

Shows which files have been modified in the working directory vs Git's staging area.

Git Add

```
git add file-name
```

Adds the new or newly modified _file-name_ to Git's staging area \(index\).

Git Commit

```
git commit -m "A really good commit message"
```

Commits all files currently in Git's staging area. The -m parameter allows for a commit message directly from the command line.

Clear!

```
clear
```

Clears all previous commands from the terminal screen -- just a bit of clean up.

Text Mate

```
mate file-name
```

All command line demos are preformed on the MacOS. Creating and editing files is done with TextMate 2 \(free\) using the **mate** command from Terminal. Passing a_file-name_to the **mate** command will create or open that file. Windows users can use the **notepad**  _**file-name**_ command instead.

---

### 17. Working Locally, Part 1  
  * Hipster Ipsum Website (hipsum. co)  

### 18. Working Locally, Part 2  

### 19. Working Locally Commands  

---
#### Git Working Locally Commands

##### Lecture Command Listing - Working Locally, Part One

```
pwd
git status
mate README.md
git status
git add README.md
git status
git commit -m "Adding some ipsum"
clear
git status
mate README.md
git status
git commit -am "Adding more ipsum"
git status
```

##### Lecture Command Listing - Working Locally, Part Two
```
pwd
git status
clear
mate index.html
git status
git add index.html
git status
mate README.md
git status
clear
git status
git add README.md
git status
git commit -m "A few changes for the website"
clear
mate README.md
mate index.html
git status
git add .
git status
git commit -m "A few more changes for website"
clear
mate README.md
git status
git add README.md
git status
git reset HEAD README.md
clear
git status
mate README.md
git checkout -- README.md
mate README.md
git status
```

##### Command Reference

Express Commit for Tracked files

```
git commit -am "Awesome commit message"
```

Use the_-a_parameter with the**git commit**command to directly commit newly modified tracked files.Warning:Only do this for small changes. Tracked files are files that have been previously added to Git \(committed or staged\).

Adding All Changed Files

```
git add .
```

The period parameter for the git add command will recursively add all new and newly modified files.

Unstage File

```
git reset HEAD file-name
```

Following the above command will "unstage" the specified file from Git's staging area \(aka index\).

Backout Working Directory Changes

```
git checkout --file-name
```

Following the above command will back out any changes made to the specified file and replace it with the version last committed in Git

---

### 20. Gitting Historical  
### 21. Removing Files  
### 22. Moving Files  
### 23. Ignoring Files  
### 24. History and File Management Commands  
---
#### Git History / File Management Commands

##### Lecture Command Listing -- History

```
git log
git help log
git log --oneline --graph --decorate --color
```

##### Lecture Command Listing -- Removing Files

```
pwd
git status
mate debug.log
ls
git status
git add .
git status
git commit -m "adding log file that really does not belong here"
clear
git status
git rm debug.log
ls
git status
git commit -m "removing log file"
clear
mate info.log
ls
git add info.log
git commit -m "adding info log"
git status
clear
ls
rm info.log
ls
git status
git add .
git add -u
clear
git status
git commit -m "Removing info.log"
```

##### Lecture Command Listing -- Moving Files

```
ls
mkdir web
ls
git mv index.html web
cd web/
ll
pwd
cd ..
ls
git status
git commit -m "Moving index.html file to web folder"
clear
```

##### Lecture Command Listing -- Ignoring Files
```
mate application.log
ls
git status
mate .iitignore
git status
ls -a
git add .gitignore
clear
git status
git commit -m "adding ignore file"
```

##### Command Reference

Seeing Repository History

```
git log
git log --oneline --graph --decorate --color
```

Git's **log** command displays the repository's history in reverse chronological order. The no-params version displays the standard view.

Git log options from above: --oneline Compacts log data on to one line, abbreviating the SHA1 hash --graph Adds asterisk marks and pipes next to each commit to show the branching graph lines --decorate Adds the markers for branch names and tags next to corresponding commits --color Adds some color to the output -- nice to have, depending on the operating system

Removing a file using Git

```
git rm file-name
```

Removing a file using Terminal

```
rm file-name
```

This removes the file outside Git's knowledge

Updating Git's Index \(staging area\)

```
git add -u
```

The_-u_parameter will recursively update Git's staging area regarding deleted/moved files outside of Git.

Making a directory \(folder\)

```
mkdir folder-name
```

The**mkdir**command is a nearly universal command for creating a directory/folder.

Making a directory \(folder\)

```
git mv source destination
```

The **git mv** command will move the_source_\(file or folder\) to the_destination_with Git.

  * 測驗3_Working with Git Locally  
