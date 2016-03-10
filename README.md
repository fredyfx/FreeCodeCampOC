# FreeCodeCampOC
Whether you are a total beginner or well experienced, we welcome you to join us if you are interested in code pairing, enhancing your technical skills in JavaScript, JQuery, HTML, CSS, Angular.js, Node.js. and much more. This is also for anyone currently taking the Free Code Camp courses online (at [www.freecodecamp.com](www.freecodecamp.com)) hoping to connect with a local campers in Orange County, CA.

## About Us
To sign up for the latest events and stay up to date with the group be sure to checkout:
* [FreeCodeCamp OC Meetup](http://www.meetup.com/Free-Code-Camp-Orange-County-CA/)
* [Facebook](https://www.facebook.com/groups/free.code.camp.orange.county/)

## Goals
* Projects to collaborate on : TBA
* Goals: Let's try to get at least one commit a day
* Download: [TeamViewer11](http://teamviewer.com/en/), [Git](https://git-scm.com/downloads)

## Getting Started with Git/GitHub
To make sure we can all contribute to this repository, make sure to download Git. There is a good guide to setting up found here: [Installing Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git). Once you have Git installed, you can run the following command to ensure it is installed:
```
git --version
```
Once installed, navigate to your working directory using the command `cd` + the name of the directory you would like to work in. For example, you could do this to navigate to the downloads folder on Mac:
```
cd Downloads
```
### Fork the repo
To contribute to this repository, you must first fork it. Click the 'fork' button at the top right of this page. This will create you own version of the repository in your GitHub account. Navigate to that page and copy the url in this box.

### Clone to your local machine
Cloning is the way Git allows us to download the repository from GitHub and put it on our local machine. To do this, copy the URL (you can click the clipboard icon on the right for a quick-copy) from your repository, and head into the Terminal/Git Client and paste in:
```
git clone https://github.com/[yourusename]/FreeCodeCampOC.git
```
This will download the folder from GitHub onto your hard drive. To navigate to the folder, type in:
```
cd FreeCodeCampOC
```
In this case, the folder will be named FreeCodeCampOC. To ensure everything worked correctly, type in:
```
git status
```
We should see the following: "On branch master. Your branch is up-to-date with 'origin/master'. Nothing to commit, working directory clean".

### Making changes
Woohoo! We made it to the fun part. To quickly add a file, type in the following:
```
echo hello world! > test.html
```
Feel free to change the text ('hello world') and the filename ('test.html'). This will add a new file to the folder, however it will not be placed in the 'staging area'. In order to save our changes, we must run:
```
git add .
```
Alternatively, you can type `git add -a`. This will add all files that you have created in this folder to the repository. If you would only like to add specific files, you can type them in, like `git add test.html`. Next up, we need to commit the changes. To do so, we can type:
```
git commit -m "my commit"
```
Notice that we can change the contents of the commit message in the quotes ("my commit"). To push changes to your GitHub repository, type in:
```
git push origin master
```
What this does is push the 'master' branch to the 'origin' remote, in which case should only be ours. See more below on remotes. What has this change done? If everything was done correctly, our forked repository should have "my commit" in the commit history. How do we merge our changes into the main FreeCodeCampOC folder? We can do so by initiating a pull request.


### Adding a remote upstream
Okay awesome, so we made some changes, contributed, went the whole mile. That's it right? Wrong. What if another person was contributing in the original FreeCodeCampOC repository, and we don't have their changes? We need to add a remote. To add a remote (this repository), type in:
```
git remote add upstream https://github.com/dinhjeffrey/FreeCodeCampOC.git
```
This will allow you to access this repo to fetch the current data. To do so, we must run:
```
git fetch upstream
git checkout master
git merge upstream/master
```
This will fetch the recent additions, and merge them with your current changes to master. For more information on this, see the links below.

## Links
* [Pull New Updates](http://stackoverflow.com/questions/3903817/pull-new-updates-from-original-github-repository-into-forked-github-repository)
* [Git Cheat Sheet](https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf)
* [Adding a remote](https://help.github.com/articles/adding-a-remote/)
* [Syncing a fork](https://help.github.com/articles/syncing-a-fork/)
