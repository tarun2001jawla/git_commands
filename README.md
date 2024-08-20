# 🚀 **Git Commands Cheat Sheet**

## 📜 **Table of Contents**
- [1. 🆕 git init](#1-git-init)
- [2. 📂 git clone](#2-git-clone)
- [3. ➕ git add](#3-git-add)
- [4. 📌 git commit](#4-git-commit)
- [5. 🔍 git status](#5-git-status)
- [6. 🚀 git push](#6-git-push)
- [7. 🔄 git pull](#7-git-pull)
- [8. 🌿 git branch](#8-git-branch)
- [9. 🔀 git checkout](#9-git-checkout)
- [10. 🔗 git merge](#10-git-merge)
- [11. 🛠️ git rebase](#11-git-rebase)
- [12. 🗂️ git stash](#12-git-stash)
- [13. 🕵️‍♂️ git reflog](#13-git-reflog)
- [14. 🔄 git reset](#14-git-reset)
- [15. ↩️ git revert](#15-git-revert)
- [16. 💾 git restore](#16-git-restore)
- [17. 🔍 git bisect](#17-git-bisect)
- [18. 🎯 git cherry-pick](#18-git-cherry-pick)
- [19. 📜 git log](#19-git-log)

---

## 1. 🆕 `git init`
- **Use**: Initializes a new Git repository.
- **Example**:
    ```bash
    git init
    ```
    This creates a `.git` directory in your project, making it a Git repository.

---

## 2. 📂 `git clone`
- **Use**: Clones an existing repository to your local machine.
- **Example**:
    ```bash
    git clone https://github.com/user/repo.git
    ```
    This command creates a copy of the repository on your local machine.

---

## 3. ➕ `git add`
- **Use**: Stages changes for the next commit.
- **Example**:
    ```bash
    git add index.html
    ```
    This stages `index.html` for the next commit.

---

## 4. 📌 `git commit`
- **Use**: Records changes to the repository.
- **Example**:
    ```bash
    git commit -m "Add index.html"
    ```
    This creates a commit with the message "Add index.html".

---

## 5. 🔍 `git status`
- **Use**: Shows the state of the working directory and the staging area.
- **Example**:
    ```bash
    git status
    ```
    This command lets you see which changes have been staged, which haven’t, and which files aren’t being tracked by Git.

---

## 6. 🚀 `git push`
- **Use**: Uploads local commits to the remote repository.
- **Example**:
    ```bash
    git push origin main
    ```
    This pushes your commits in the `main` branch to the remote repository.

---

## 7. 🔄 `git pull`
- **Use**: Fetches changes from a remote repository and merges them into the current branch.
- **Example**:
    ```bash
    git pull origin main
    ```
    This command updates your current branch with the latest changes from the remote repository.

---

## 8. 🌿 `git branch`
- **Use**: Lists, creates, or deletes branches.
- **Example**:
    ```bash
    git branch feature-branch
    ```
    This creates a new branch called `feature-branch`.

---

## 9. 🔀 `git checkout`
- **Use**: Switches branches or restores working tree files.
- **Example**:
    ```bash
    git checkout feature-branch
    ```
    This switches to the `feature-branch`.

---

## 10. 🔗 `git merge`
- **Use**: Merges branches.
- **Example**:
    ```bash
    git merge feature-branch
    ```
    This merges the `feature-branch` into the current branch.

---

## 11. 🛠️ `git rebase`
- **Use**: Reapplies commits on top of another base tip.
- **Example**: 
    ```bash
    git rebase main
    ```
    This moves the current branch to start at the tip of the `main` branch.

### Interactive Rebase (`git rebase -i`)
- **Use**: Clean up your commit history by squashing, editing, or re-ordering commits.
- **Example**:
    ```bash
    git rebase -i HEAD~4
    ```
    An interactive rebase allows you to squash, edit, or reorder the last 4 commits.

---

## 12. 🗂️ `git stash`
- **Use**: Temporarily saves changes that aren't ready to be committed.
- **Example**:
    ```bash
    git stash
    ```
    This stashes your uncommitted changes, allowing you to work on something else.

    ```bash
    git stash pop
    ```
    This re-applies the stashed changes.

---

## 13. 🕵️‍♂️ `git reflog`
- **Use**: Tracks updates to the tip of branches and allows you to recover lost commits.
- **Example**:
    ```bash
    git reflog
    ```
    This shows the history of the HEAD pointer, helping you recover lost commits.

---

## 14. 🔄 `git reset`
- **Use**: Resets the current branch to a specific state.
### Types of Reset:
- **Soft**: Moves the HEAD but keeps the changes staged.
    ```bash
    git reset --soft HEAD~1
    ```
- **Mixed**: Moves the HEAD and unstages the changes.
    ```bash
    git reset --mixed HEAD~1
    ```
- **Hard**: Moves the HEAD and discards all changes.
    ```bash
    git reset --hard HEAD~1
    ```

---

## 15. ↩️ `git revert`
- **Use**: Creates a new commit that undoes the changes of a specific commit.
- **Example**:
    ```bash
    git revert c9e2b4d
    ```
    This command will undo the changes from commit `c9e2b4d` by creating a new commit.

---

## 16. 💾 `git restore`
- **Use**: Restores working tree files.
- **Example**:
    ```bash
    git restore index.html
    ```
    This restores `index.html` to its state in the last commit.

---

## 17. 🔍 `git bisect`
- **Use**: Finds the commit that introduced a bug by performing a binary search through your commit history.
- **Example**:
    ```bash
    git bisect start
    git bisect bad  # Mark current commit as bad
    git bisect good c9e2b4d  # Mark known good commit
    ```
    This starts the bisect process, narrowing down the commit that introduced the bug.

---

## 18. 🎯 `git cherry-pick`
- **Use**: Apply specific commits from one branch to another.
- **Example**:
    ```bash
    git cherry-pick c9e2b4d
    ```
    This command applies the changes from commit `c9e2b4d` to your current branch.

---

## 19. 📜 `git log`
- **Use**: Shows the commit history.
- **Example**:
    ```bash
    git log --oneline
    ```
    This shows the commit history in a condensed format, one commit per line.

---

### **📝 Summary**
By mastering these Git commands, you'll have the tools you need to manage your projects effectively. Use this cheat sheet as a reference to improve your workflow and Git proficiency.
