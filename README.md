"# github-3.2-soon" 

# A. GitHub Authentication Methods

GitHub Authentication refers to the various ways that GitHub can confirm your identity before you can access repositories/data/files on GitHub. When you authenticate to GitHub, you supply or confirm credentials that are unique to you to prove that you are exactly who you declare to be.

GitHub provides 3 modes of authentication:
- Username and password with two-factor authentication.
- Personal access token.
- SSH key.

# B. 16 commonly used Git commands every developer should know.

## 1. git add

### 1.1 Usage

This command adds file(s) to the "staging area".

Files in the staging area are tracked by Git.

When you next run git commit, all files in the staging area are uploaded to the remote repository.

### 1.2 Example command(s)

The command allows you to add file(s) to the staging area. After the git add command is run, the files you specified become tracked file(s) and Git will monitor the changes in these files if there are any conflicting changes made by others in the remote repository.

``` sh
git add <one_or_more_file_to_add>
```

## 2. git branch

### 2.1 Usage

This command lists the local branch names.

If you add the -r parameter, Git shows you the remote branches:

You can also use git branch to delete a branch by adding the -d parameter before the branch name:

### 2.2 Example command(s)

``` sh
git branch

git branch -r
output:
origin/HEAD
origin/master

git branch -d <branch_name_to_delete>
```


## 3. git cat-file

### 3.1 Usage

Thie command provides contents or details of repository objects.

### 3.2 Example command(s)

``` sh
git cat-file -p <commit_hash>
```


## 4. git checkout

### 4.1 Usage

This command is used to switch to the branch that you want to work on.

### 4.2 Example command(s)

``` sh
git checkout <branch_to_switch_to>

```


## 5. git clean

### 5.1 Usage

This command is used to remove untracked files from your working tree.

### 5.2 Example command(s)

``` sh
git clean
```


## 6. git clone

### 6.1 Usage

This command creates a complete copy, or a clone, of a remote repository.

### 6.2 Example command(s)

``` sh
git clone <URL_of_remote_repository>
```


## 7. git config

### 7.1 Usage

Use this command to specify the configuration settings of Git (the config file is stored in .git/config).

### 7.2 Example command(s)

``` sh
git config
git config --global user.name "your_github_user_name"
git config --global user.email "your_github_user_id@gmail.com"
git config --global color.ui "auto"
```


## 8. git commit

### 8.1 Usage

This command creates a commit. Commits are the individual pieces of history stored by the repository. Each one marks the progression of the changes you made over time.

Use more than one -m option if you have multiple commit messages to type.

### 8.2 Example command(s)

``` sh
git commit -m <commit_message>

git commit -m "Subject: what I changed" -m "Body: why I changed it"
```


## 9. git fetch

### 9.1 Usage

This command updates your remote branches; it doesn’t merge the changes into your local branch.

### 9.2 Example command(s)

``` sh
git fetch
```


## 10. git init

### 10.1 Usage

To convert or make the current directory (folder where git init is run) a working directory.

### 10.2 Example command(s)

``` sh
git init
```


## 11. git pull

### 11.1 Usage

 You can use git pull if you want to fetch changes from a remote repository and merge them into your local branch at the same time.

### 11.2 Example command(s)

``` sh
git pull
```


## 12. git push

### 12.1 Usage

Getting changes from upstream repositories is only half of keeping in sync with everyone else on your team. Use git push if you need to be able to push changes back to an upstream repository to share the changes with everyone else.

### 12.2 Example command(s)

``` sh
git push
```


## 13. git remote

### 13.1 Usage

Use the git remote command to create, remove, manipulate, and view a remote branch name. All the remotes you introduce are recorded in the .git/config file
and can be manipulated using git config.

### 13.2 Example command(s)

``` sh
git remote -v
output:
origin  https://github.com/username/sample-app.git (fetch)
origin  https://github.com/username/sample-app.git (push)
```


## 14. git revert

### 14.1 Usage

Use git revert to undo the effects of a commit that is buried, perhaps deeply, in the history of a branch.

### 14.2 Example command(s)

``` sh
git revert <commit_hash>
```


## 15. git status

### 15.1 Usage

This command provides information, such as which files are untracked, which are tracked and what their changes are, which is the current “branch”, and what the status of the current branch is with respect to a “remote”.

This command should indicate that there are no outstanding changes to be committed if you did not add/update/delete any files in the working directory.

### 15.2 Example command(s)

``` sh
git status
```


## 16. git switch

### 16.1 Usage

This is a new command introduced in Git version 2.23.0.

This command allows you to switch to a specific branch in your repository.

### 16.2 Example command(s)

``` sh
git switch <branch_to_switch_to>
```

# C. The 4 Github commands that I will likely use the most in the real projects are undoubtedly:
  - git add
  - git commit
  - git push
  - git pull

Because these commands are the ones that allow us to synchronise the local repository with the remote repository.

## <font color='lightgreen'>References:</font>
- [Cheat Sheet – 50 Git Commands You Should Know](https://www.freecodecamp.org/news/git-cheat-sheet/)
- [Git - Reference](https://git-scm.com/docs)
- [GIT CHEAT SHEET - GitHub Education](https://education.github.com/git-cheat-sheet-education.pdf)