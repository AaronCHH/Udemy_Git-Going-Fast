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
  * 測驗4_Going Remote  
