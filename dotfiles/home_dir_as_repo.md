### home directory as git repo for easy dotfiles management

- First, set up the home directory as a git repo with a .gitignore that ignores everything.

```
cd ~
git init
echo "*" >> .gitignore
```

- Force add individual configuration files which will then track changes on those files only.

```
git add -f .vimrc
```

- Commit the home repo and push it up to Github, etc. 

```
you know what to do
```

- On the new machine, pull down the repo and resume where you left off.

*** DREW DEVAULT'S SOLUTION ***
```
cd ~
git init
git remote add origin git@github.com:arntzy/home.git
git fetch
git checkout -f master
```
