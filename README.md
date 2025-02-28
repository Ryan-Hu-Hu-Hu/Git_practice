# My git practicing

IMPORTANT
Please create a new repository first!


Create a new folder and let it initailized by git
```
mkdir Git_practice 
cd Git_practice
git init
```
Create a README file in markdown syntax 
```
echo "First git practicing" > README.md
```
After this, all the description and the codes will be recorded in  README.md 

Check git status, whether it has been modified or need to be committed 
```
git status
```
At initial, the file status is "Untracked" or "U", and after any modification, it will become "Modified" or "M"


Let git start to track the README.md file
```
git add README.md
```
At this stage, the file will be added into "Staging Area", and the status becomes "new file" or "A" 

If you modify multiple files and want to add all the files into staging area, use:
```
git add -all
```
Before commit, make sure the configuration is set to your git account
```
git config user.email "your Github mail"
# or  git config user.name "your Github name"
```

Let the temporary files in staging area become permanent storage
```
git commit -m "init commit"
```
-m and the following words in "" states the comment of what you did in this commit

Connect with the remote github server
```
git remote add origin https://github.com/your_account_name/your_branch_name.git
# The defult branch name is master, so chaning name to main is optional  
git branch -M main
# If using "master", then change the following "main" to "master"
git push -u origin main
```

If pushing to your own fork from other's repository, change the remote url to your own github first
```
git remote set-url origin https://github.com/YOUR_GITHUB_NAME/YOUR_FORK.git
git push -u origin main
```
Then you can successfully push to your own fork


Reference 
1. https://gitbook.tw/chapters/using-git/init-repository
2. https://gitbook.tw/chapters/using-git/add-to-git
3. https://gitbook.tw/chapters/github/push-to-github
4. https://docs.github.com/en/get-started