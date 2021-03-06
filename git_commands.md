# Commonly used git commands

## ***The Fundamentals***

**Create repository:**
```
git init
```

**Add changed files to be commited:**
```
git add -A
```

**Commit changes:**
```
git commit -m "some message"
```

**Add a remote to push to / pull from:**
```
git remote add <remote name (often "origin")> <URL of remote repository (https://github.com/...)>
```

**Set an upstream and push to the remote repo:**

Only use this the first time you push.
```
git push -u <remote name> <remote branch name> 
```

After that, you only need this to push.
```
git push
```

**Pull from remote repository:**

This only works if you have the upstream set.
```
git pull
```

---

## ***Going Deeper***

**View list of local branches and see what branch you are currently on:**

The branch with a **\*** next to it is the one you are currently on. If this command takes you out of the command line, press the **q** key to return to it.
```
git branch
```

**Create a new branch and switch to it:**
```
git checkout -b <branch name>
```

**Create a new branch without switching to it:**
```
git branch <branch name>
```

**Switch to an existing branch:**
```
git checkout <branch name>
```

**Delete an existing branch:**

You cannot delete the branch you are currently on.
```
git branch -d <branch name>
```

**View commit history:**

If this takes you out of the command line, press the **q** key to return to it.
```
git log
```

**Switch to a previous commit:**

To return to the latest commit, checkout the branch it belongs to.
```
git checkout <commit ID>
```

**Clone a remote repository to your local machine:**

Leave the second argument empty to clone it into the current directory.
```
git clone <URL of repository> <directory you want the repo in>
```

**View changes you've made since the previous commit:**

Run this to view what files have changed.
```
git status
```

Run this to view the changes within those files. This only works before you stage the changes with `git add -A`
```
git diff
```

If you've already staged the changes, run this.
```
git diff --staged
```

```diff
+Green represents lines that have been added
-Red represents lines that have been removed
```

If these commands take you out of the command line, press the **q** key to return to it.

**Revert files back to the latest commit:**
```
git reset --hard
```
