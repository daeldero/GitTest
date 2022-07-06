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

# Now, the contents of this md. file is changed

### Check the status of Git worktree
```
git status
git status -s
```
* File status
  * *Untracked* file: File ever uncommited
  * *Staged* file: File added in local repository (stage)
  * *Unmodified* file: Commited file without any modification after commit
  * *Modified* file: Commited file with modification after commit

### Add and commit the modified file
```
git commit -am "< description_about_this_update >"
```
* '-a' or '-am' is not allowed for untracked file.

### Check the history of commits
```
git log
git log -< number >
git log --oneline
```
* '-*number*' option shows only *number* commits.
* '--oneline' option shows commit message in short.

```
git checkout < first_7_numbers_of_commit >
git checkout -
```
* 'checkout' switch commits (or branches).
* '-' option means the latest commit.
- - -
