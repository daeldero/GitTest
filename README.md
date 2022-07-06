# First commit

### Start Git: Generate a local repository
```
git init
```
* **Local repository** means '.git' folder in local PC.
* **Remote repository** means repository in GitHub.
* **Git repository** means local repository in a narrow sense, or working directory in a wide sense.
* **Worktree** roughly means working directory, and precisely complement parts of local repository from working directory.
  * In other words, working directory = working tree + local repository

### Set configuration
```
git config --global user.email "< my_email@gmail.com >"
git config --global user.name "< my_name >"
git config --list
```

### Add: Staging - add file to stage
```
git add < files > 
git add .
```
* The last '.' of second line means all files in the directory.
* Before *add*, the status of corresponding file is *untracked*.
* After *add*, the status of the file is converted to *staged*.

### Commit: Update git - move staged files to local repository
```
git commit -m "< description_about_this_commit >"
git commit -a
git commit -am "< description_about_this_commit >"
```
* '-m' option means message that describes about this commit.
* '-a' option means *add* that performs *add* and *commit* at once.
* '-am' = '-a' + '-m'
- - -
