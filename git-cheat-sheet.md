
# 📝 Git Cheat Sheet (Education Edition)

Git is a **free and open-source distributed version control system** that allows you to **track changes**, **collaborate**, and **manage source code** efficiently. This cheat sheet summarizes the most commonly used Git commands.

---

## 🔧 Setup & Configuration

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
git config --global color.ui auto
```

- Sets your name and email for commits.
- Enables colored output for readability.

---

## 🆕 Initialize & Clone

```bash
git init
git clone [url]
```

- `git init`: Initialize a Git repository in your current directory.
- `git clone`: Copy an existing repository from a URL (e.g., GitHub).

---

## 📂 Staging & Snapshots

```bash
git status
git add [file]
git reset [file]
git diff
git diff --staged
git commit -m "Your message"
```

- `git status`: Check which files are modified or staged.
- `git add`: Stage a file for commit.
- `git reset`: Unstage a file, keeping changes.
- `git diff`: Show unstaged changes.
- `git diff --staged`: Show staged changes.
- `git commit`: Save staged changes as a snapshot.

---

## 🌿 Branching & Merging

```bash
git branch
git branch [branch-name]
git checkout [branch-name]
git merge [branch-name]
git log
```

- `git branch`: List branches.
- `git checkout`: Switch to another branch.
- `git merge`: Merge a branch into the current branch.
- `git log`: View commit history.

---

## 🔄 Share & Update

```bash
git remote add [alias] [url]
git fetch [alias]
git merge [alias]/[branch]
git push [alias] [branch]
git pull
```

- `git remote add`: Add a remote repository.
- `git fetch`: Download all branches from the remote.
- `git merge`: Merge a remote branch into your local one.
- `git push`: Send local commits to the remote.
- `git pull`: Fetch and merge from remote.

---

## 🗂 Tracking Path Changes

```bash
git rm [file]
git mv [old-path] [new-path]
git log --stat -M
```

- `git rm`: Remove file and stage for deletion.
- `git mv`: Rename or move files.
- `git log --stat -M`: Show moved/renamed paths in commit logs.

---

## 💾 Stashing (Temporary Saves)

```bash
git stash
git stash list
git stash pop
git stash drop
```

- `git stash`: Save changes temporarily.
- `git stash list`: View stashes.
- `git stash pop`: Reapply and remove the last stash.
- `git stash drop`: Delete the latest stash.

---

## 🧽 Rewriting History

```bash
git rebase [branch]
git reset --hard [commit]
```

- `git rebase`: Reapply commits from current branch onto another.
- `git reset --hard`: Reset to a specific commit and discard all changes.

---

## 🔍 Inspect & Compare

```bash
git log
git log branchB..branchA
git log --follow [file]
git diff branchB...branchA
git show [SHA]
```

- `git log`: Show commit history.
- `branchB..branchA`: Commits in A but not in B.
- `--follow`: Track file history through renames.
- `diff A...B`: Show differences between branches.
- `show [SHA]`: Show detailed info for a commit or object.

---

## 🚫 Ignoring Files

```bash
.gitignore
```

Create a `.gitignore` file and add patterns:

```gitignore
logs/
*.notes
pattern*/
```

To apply globally:

```bash
git config --global core.excludesfile [path/to/file]
```

---

## 🖥 GUI & Installation Resources

- GitHub for Windows: https://windows.github.com  
- GitHub for Mac: https://mac.github.com  
- Git for All Platforms: https://git-scm.com  

---

## 🎓 GitHub for Education

- Free for students and teachers.
- Discounts for educational use.  
- Learn more: [education.github.com](https://education.github.com)  
- Contact: education@github.com

---

✅ **Pro Tip**: Use `--help` after any Git command to see its usage.  
Example: `git commit --help`
