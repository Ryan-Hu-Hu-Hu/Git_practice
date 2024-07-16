First git practicing

Create a new folder and let it initailized by git
```
mkdir Git_practice 
cd Git_practice
git init
```
Create a Note file in markdown syntax 
```
echo "First git practicing" > Notes.md
```
After this, all the description and the codes will be recorded in  Notes.md 

Check git status, whether it has been modified or need to be committed 
```
git status
```
At initial, the file status is "Untracked" or "U", and after any modification, it will become "Modified" or "M"


Let git start to track the Note.md file
```
git add Note.md
```
At this stage, the file will be added into "Staging Area", and the status becomes "new file" or "A" 

If you modify multiple files and want to add all the files into staging area, use:
```
git add -all
```

Let the temporary files in staging area become permanent storage
```
git commit -m "init commit"
```
-m and the following words in "" states the comment of what you did in this commit

Reference 
1. https://gitbook.tw/chapters/using-git/init-repository
2. https://gitbook.tw/chapters/using-git/add-to-git
3. https://gitbook.tw/chapters/github/push-to-github