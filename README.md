# 5-Minutes-to-Learn-GitHub-Basic-with-Git

*If you want to reprint this article, please label its origin "https://github.com/ZhaiJojo/5-Minutes-to-Learn-Github-Basic-with-Git/" explicitly.*

This is a very quick guide to make you use GitHub as an online code container in Windows 10. All procedures in this guide are the easiest way among all ways that I can think of to do the same things.

## Basic Things 

### How to upload your local projects to GitHub?

Install Git form [its official website](https://git-scm.com/). Leave all installation settings as default.

Enter your local directory with Windows file browser where you store your code, for example, D:\project1.

Sign in to your GitHub, create a new repository called “project1”, leaving all settings as default.

Right click an empty area and choose "Git Bash Here"

Enter these commands in order:
```
git init

git add .

git commit -m “your commit message”

git remote add origin [URL of project1 in GitHub]

git push origin master
```
Finished! If you want to add a README in your project, just new a “README.md” file in your project folder before you enter those commands. GitHub can recognize it automatically according to its filename and display the content of “README.md” in your online repository. Notice! Do not edit the “README.md” with the Windows embedded notepad, otherwise some garbled characters may be display in your online repository. Notepad ++ is recommended.

### How to update your online repository?

If you have edited the files in your local “project1” folder and want to update your online repository, you should enter these commands in the Git Bash opened with the same manner as before:
```
git add .

git commit -m “your commit message”

git push origin master
```
### How to download your online repository to local?

You should enter these commands in the Git Bash opened with the same manner as before:
```
git pull origin master --allow-unrelated-histories
```

## Advanced skills

If you want to use git and GitHub as a version control tool, not just a tool to upload and download your codes, there is a must to learn something more hard and more interesting. Now this section is not complete, I will refine it later.

### “Merge” command

get all the different things from another branch. When there are collisions, git will enter merge state automatically and you have to merge it manually.

### Push failure

When you want to push, the branch online must be the ancestor of your local branch pushed. If not, you should pull it first.

