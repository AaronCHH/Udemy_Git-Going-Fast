## Ch04_Going Remote

<!-- toc orderedList:0 depthFrom:1 depthTo:6 -->

- [Ch04_Going Remote](#ch04_going-remote)
	- [25. Setting Up SSH Authentication](#25-setting-up-ssh-authentication)
	- [26. SSH Authentication Commands](#26-ssh-authentication-commands)
		- [SSH Authentication Commands](#ssh-authentication-commands)
			- [Lecture Command Listing](#lecture-command-listing)
			- [Command Reference](#command-reference)
	- [27. Collaborating with Others -- Git Remotes and   GitHub](#27-collaborating-with-others-git-remotes-and-github)
	- [28. Git Remote Commands](#28-git-remote-commands)
		- [Git Remote Commands](#git-remote-commands)
			- [Lecture Command Listing](#lecture-command-listing-1)
			- [Command Reference](#command-reference-1)

<!-- tocstop -->

### 25. Setting Up SSH Authentication  
  * GitHub website (github. com)    


### 26. SSH Authentication Commands  
---
#### SSH Authentication Commands

##### Lecture Command Listing

```
cd ~
cd .ssh
mkdir .ssh
cd .ssh
pwd
ssh-keygen -t rsa -C "jason@jasongtaylor.com"
mate id_rsa.pub
ssh -T git@github.com
```

##### Command Reference

Generating an SSH Key

```
ssh-keygen -t rsa -C "your.name@your-company.com"
```

Use your actual email address in the example above.

Verify SSH authentication

```
ssh -T git@github.com
```

Above command uses **ssh** to connect to GitHub over the SSH protocol.

---

### 27. Collaborating with Others -- Git Remotes and   GitHub
  * GitHub website (github. com)  

### 28. Git Remote Commands  
---
#### Git Remote Commands

##### Lecture Command Listing

```
git status
git remote add origin git@github.com:scm-ninja/git-demo.git
git remote -v
git push -u origin master
git push origin master
ls
cd web/
mate index.html
clear
git commit -am "Updating index page for GH"
git status
git pull origin master
git push origin master
```

##### Command Reference

Creating a remote repository reference

```
git remote add remote-name remote-repository-location
```

Using **git remote add** command allows us to associate a remote repository. Normally, you want to paste in the full URL for the remote repository given to you by your Git host \(GitHub\). By convention, the first or primary remote repository is named_origin_.

List Git's Remotes

```
git remote -v
```

The **git remote** command lists the names of all the remote repositories and the -v parameter \(verbose\) will display the full URL of the remote repository for each remote name listed

Send Changes to Remote

```
git push -u remote-name branch-name
git push remote-name branch-name
```

The **git push** sends all your local changes \(commits\) on branch _branch-name_ to the remote named _remote-name_. The **-u** parameter is needed the first time you push a branch to the remote.

Receive Changes from Remote

```
git pull remote-name branch-name
```

The **git pull** receives all your remote changes \(commits\) from the remote named _remote-name_ and on branch _branch-name_ .

---
  * 測驗4_Going Remote  
