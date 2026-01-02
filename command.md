

# git commands Remove-Item -Recurse -Force .git
# git config --global user.name "Your Name"
# git config --global user.email "your@email.com"
# git config --global core.editor "code --wait"
# git config --global init.defaultBranch main
# git config --global pull.rebase true
# git config --global alias.cm commit
# git config --global alias.unstage "restore --staged"

# u = untracted , A = Added , C = Commited:

# git init
# Remove-Item -Recurse -Force .git   # Windows PowerShell or rm -rf .git    
 <!-- git config --global -e -->
# 
# git config --global --reset user.name
# git config --global --reset user.email
# git config --global --reset core.editor
# git config --global --reset init.defaultBranch
# git config --global --reset pull.rebase
# git config --global --reset alias.cm
# git config --global --reset alias.unstage
# git add .
# git commit -m "Initial commit"
# git remote add origin
# git branch -M main
# git push -u origin main
# git pull origin main
#   
# git clone <repository_url>
# git status
# git add <file_name>

 <!-- git help -->
#  git help commit
hii gise  

# git diff command cle
git diff
then 
git diff --staged 

# git commit command
git clean command 
# git clean -n , git clean -f is used to  remove the untracted file like any file is not tracted or added by git git add it will be removed automatically bny git clean -f = flush git clean -fd for direactory 
git rename 
git move file command
git undo commit 
git undo 
git stages 
to create a file we use ==  New-Item padai.py

5f31a11 (HEAD -> main) important
ab4c435 ok
e9fca31 Add git command reference note3
219943b Add git command reference note2
1eba574 (master) Add git command reference note1
b239e3b Add git command reference notes
PS C:\Users\Sarthak jain\Desktop\git>  so 5f31 is commit id 
git show 6caf30a is used to check the git commit  history 

> git log --oneline is used to check all the checkpoint done 

how to undo the git = git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD~1


git revert commit id 

# Now starting with the 🌿 Git Branch Commands – FULL GUIDE
# 1. View Branches
# git branch    
<!-- List all remote branches
git branch -r -->


List local + remote branches
git branch -a or git branch 
Create Branches
▶ Create a new branch
git branch feature1

Create and switch (old way)
git checkout -b feature1

Create and switch (modern & recommended)
git switch -c feature1


1. Rename Branch
▶ Rename current branch
git branch -m new-name

▶ Rename another branch
git branch -m old-name new-name

Delete Branches
▶ Delete local branch (safe)
git branch -d feature1
Merge Branches
▶ Merge another branch into current branch
git merge feature1
git switch main
git merge feature1
Abort a merge (if conflict)
git merge --abort

7. Compare Branches
▶ See commits in one branch not in another
git log main..feature1

 8. Track Remote Branches
▶ Create local branch tracking remote
git checkout -b feature1 origin/feature1

Remote Repository Commands (GitHub)
git remote -v
git remote add origin <url>
git remote remove origin
git remote rename old new

git push origin main
git push -u origin main
git pull origin main
git fetch origin


# complete Here is a **complete, structured list of Git commands**, from **basic to advanced**, useful for **college exams, interviews, and real-world development**.
(Perfect for you since you’re already learning Git & GitHub 👍)

---

# 🔹 1. Git Configuration Commands

Used once or rarely.

```bash
git config --global user.name "Your Name"
git config --global user.email "you@email.com"
git config --global --list
git config --system --list
git config --local --list
```

---

# 🔹 2. Repository Creation & Initialization

```bash
git init                # Initialize a new repository
git clone <url>         # Clone a remote repository
git clone <url> <dir>   # Clone into specific folder
```

---

# 🔹 3. Working Directory & File Management

```bash
git status              # Check repository status
git add file.txt        # Stage a file
git add .               # Stage all files
git add -A              # Stage all changes
git rm file.txt         # Delete file and stage deletion
git mv old new          # Rename/move file
```

---

# 🔹 4. Commit Commands

```bash
git commit -m "message"
git commit              # Opens editor
git commit -a -m "msg"  # Add & commit tracked files
git commit --amend      # Modify last commit
```

---

# 🔹 5. Branching Commands

```bash
git branch              # List branches
git branch new-branch   # Create branch
git branch -d branch    # Delete branch
git branch -D branch    # Force delete branch

git checkout branch     # Switch branch
git checkout -b branch  # Create & switch branch

git switch branch
git switch -c branch
```

---

# 🔹 6. Merging & Rebasing

```bash
git merge branch        # Merge branch into current
git merge --abort       # Abort merge

git rebase branch       # Rebase current branch
git rebase --abort
git rebase --continue
```

---

# 🔹 7. Remote Repository Commands (GitHub)

```bash
git remote -v
git remote add origin <url>
git remote remove origin
git remote rename old new

git push origin main
git push -u origin main
git pull origin main
git fetch origin
```

---

# 🔹 8. Log & History Commands

```bash
git log
git log --oneline
git log --graph
git log --decorate
git show <commit-id>
```

---

# 🔹 9. Undo & Recovery Commands (VERY IMPORTANT)

```bash
git restore file.txt
git restore --staged file.txt

git reset --soft HEAD~1
git reset --mixed HEAD~1
git reset --hard HEAD~1

git revert <commit-id>
git reflog
```

---

# 🔹 10. Stash Commands

```bash
git stash
git stash list
git stash apply
git stash pop
git stash drop
git stash clear
```

---

# 🔹 11. Diff & Comparison

```bash
git diff
git diff --staged
git diff branch1 branch2
git diff commit1 commit2
```

---

# 🔹 12. Tagging Commands

```bash
git tag
git tag v1.0
git tag -a v1.0 -m "version 1.0"
git push origin v1.0
git tag -d v1.0
```

---

# 🔹 13. Git Ignore

```bash
.gitignore
```

Example:

```
__pycache__/
.env
*.log
```

---

# 🔹 14. Submodules (Advanced)

```bash
git submodule add <url>
git submodule init
git submodule update
```

---

# 🔹 15. Git Clean (Dangerous ⚠️)

```bash
git clean -n     # Dry run
git clean -f     # Delete untracked files
git clean -fd    # Delete untracked files & folders
```

---

# 🔹 16. Help Commands

```bash
git help
git help commit
git commit --help
```

---

# 🔹 17. Shortcuts & Aliases

```bash
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
```

---

# 🔹 18. Complete Common Workflow (Interview Favorite)

```bash
git init
git add .
git commit -m "initial commit"
git branch -M main
git remote add origin <url>
git push -u origin main
```

---

## ✅ If you want next:

* 📘 **Git commands explained with examples**
* 🧠 **Git interview questions**
* ⚔️ **Git vs GitHub**
* 🗂️ **Real project Git workflow**
* 🧪 **Git practice problems**

Just tell me 👍

