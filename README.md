# Commands

## Remote (New repo):
```
git init
git remote add origin https://github.com/your-user/your-repo.git
git remote -v
git branch -M main
git add .
git commit -m "some message"
git push -u origin main
```

## Remote (Existing repo):
```
git init
git remote add origin https://github.com/your-user/your-repo.git
git remote -v
git pull origin main
```

## Branches:
```
git checkout main
git checkout another_branch
```

## Merge a branch with Master:
```
git fetch origin master:master
git merge master
```

## Delete:
```
rm -rf .git
```

## User Setup:
```
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
git config --global init.defaultBranch main
```

## In .gitconfig file do:
```
sudo nano ~./gitconfig
[init]
        defaultBranch = main
 
[credential]
        helper = store
```

## Gitignore:
.gitignore:
```
git rm --cached <file or directory to be removed> //remove file to ignore
```
1. make .gitignore file.
2. add node_modules/ line to gitignore file
3. run this command
	```
	git rm -r --cached .
	git add .
	git commit -m "remove gitignore files"
	git push
	```
