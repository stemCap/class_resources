# Commonly used git commands

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