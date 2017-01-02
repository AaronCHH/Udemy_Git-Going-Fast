## Ch02_Setup and Configuration

<!-- toc orderedList:0 depthFrom:1 depthTo:6 -->

- [Ch02_Setup and Configuration](#ch02_setup-and-configuration)
	- [5. Setup Overview](#5-setup-overview)
	- [6. Installing Git for Windows](#6-installing-git-for-windows)
	- [7. Installing Git on a Mac via the Command Line](#7-installing-git-on-a-mac-via-the-command-line)
	- [8. Gitting Help](#8-gitting-help)
	- [9. Help Commands](#9-help-commands)
			- [Git Help Commands](#git-help-commands)
			- [Lecture Command Listing](#lecture-command-listing)
			- [Command Reference](#command-reference)
	- [10. Git Configuration](#10-git-configuration)
	- [11. Configuration Commands](#11-configuration-commands)
		- [What's the current directory \(present working directory\)?](#whats-the-current-directory-present-working-directory)
		- [Git Config \(Global/User-level\) Syntax](#git-config-globaluser-level-syntax)
		- [Configure User and Email](#configure-user-and-email)
		- [Listing All Global Configuration Settings](#listing-all-global-configuration-settings)
		- [Seeing Git's User-based Config file](#seeing-gits-user-based-config-file)

<!-- tocstop -->

### 5. Setup Overview  
  * Git For Windows dowlnoad (git-scm. com)    

### 6. Installing Git for Windows  

### 7. Installing Git on a Mac via the Command Line  

### 8. Gitting Help  

### 9. Help Commands  
---

##### Git Help Commands
Help commands here  

##### Lecture Command Listing

```
git help
git help config
```

##### Command Reference

Getting general help:

```
git help
```

Help Command Syntax -- getting help about a specific Git command:

```
git help command
```
---

### 10. Git Configuration  

### 11. Configuration Commands  
---
#### What's the current directory \(present working directory\)?

```
pwd

```

#### Git Config \(Global/User-level\) Syntax

```
git config --global
setting
value
```

#### Configure User and Email

General Syntax:

```
git config --global user.name "Your Name"
git config --global user.email "you@someplace.com"

```

Example using course author's information:

```
git config --global user.name "Jason Taylor"
git config --global user.email "jason@jasongtaylor.com"

```

#### Listing All Global Configuration Settings

```
git config --global --list

```

#### Seeing Git's User-based Config file

```
cat ~/.gitconfig
```


  * 測驗2_Setup and Configuration  
