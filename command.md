

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