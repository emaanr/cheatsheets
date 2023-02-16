# Git

    Git Cheatsheet.

# Table on Contents

- [Git](#git)
- [Table on Contents](#table-on-contents)
- [Create New Repo via CLI](#create-new-repo-via-cli)
  - [Pre-Requisites](#pre-requisites)
  - [Steps](#steps)

# Create New Repo via CLI

    How to take any folder, turn it into a git repository, and push to GitHub repo of the same name.

## Pre-Requisites

- Make sure there is a newly initialized and empty repository with the same name as the folder you wish to push.

## Steps

1. `git init`
   - Initialize repository, this creates a `.git` folder in the project's root folder (whose name should be the same as the repo you are trying to push to).
2. `git add .`
   - Add all files to be staged for commit.
3. `git commit -m "MESSAGE"`
   - Commit staged files with commit message, MESSAGE.
4. `git branch -M main`
   - This branch renames the default branch name `master` to `main` via the use of the `-M` flag.
   - I prefer to use `main` over `master`, otherwise this step could be skipped entirely.
5. `git remote add origin https://github.com/USERNAME/REPO-NAME`
   - To tell the local git repository on your computer which remote repository to send changes to.
6. `git push -u origin main`
   - The `-u` flag adds a tracking reference to the upstream server you are pushing to.
   - This means that every next push/pull done from within our local repository will know to send/retrieve information to/from the `main` branch.
   - Recall that if you didn't do `Step 4` then you would instead invoke `git push -u origin master` at this point.
