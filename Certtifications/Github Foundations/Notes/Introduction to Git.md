---
sticker: lucide//git-pull-request
---

Version Control System -> VCS


## Configure Git

- Once installing Git you can check the version of git you are on by doing
```
git --version
```

	this should return `git version 2.7.4`

### Define Global Variables

- To initialize configuring git we should define the global variables `user.name` and `user.email`
	- This is required to make commits to do this you do:
```
git config --global user.name "<User_Name>"
```

```
git config --global user.email "<User_EMAIL>"
```

- To Check what the global variables are you do: 
```
git config --list 
```
You should get an output like this 
`user.name=User Name`
`user.email =user-name@gmail.com`

## Set Up Git Repo (Manually)

1. Set the Directory

```
mkdir <Folder Name>
```

2. Change the project direcotry by using the cd command:

```
cd <Folder Name>
```

3. To initialize the new repository and set the name of the default branch to `main`"

```
git init --initial-branch=main
```

or use 

```
git init -b main
```

You should get an output like this:

```
OUTPUT:
Initialized empty Git repository in /home/<user>/repo/.git/ Switched to a new branch 'main'
```

4. Use `git status` command to show the status of the working tree

```
git status
```

GIT REESPONDS WITH:

```
On branch main
No commits yet
```

5. Use an `ls` command to show the contents of the working tree:
```
ls -a
```

