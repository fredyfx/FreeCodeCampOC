# FreeCodeCamp/OrangeCounty
Welcome to the [Free Code Camp](www.freecodecamp.com) Orange County community repo!

[![Join the chat at https://gitter.im/FreeCodeCamp/OrangeCounty](https://img.shields.io/badge/GITTER-join%20chat-green.svg)](https://gitter.im/FreeCodeCamp/OrangeCounty)

## About Us
Whether you are a total beginner or an experienced developer, join us to grow your skills in HTML, CSS, and JavaScript. If you haven't already, be sure to join our local [Meetup](http://www.meetup.com/Free-Code-Camp-Orange-County-CA/) to receive updates and invites to connect with other Orange County campers. You can also into or join the [Facebook Group](https://www.facebook.com/groups/free.code.camp.orange.county/) or pop into [our chat room](https://gitter.im/FreeCodeCamp/OrangeCounty) to introduce yourself or get help.

Experienced devs are welcome too! What better way to hone your skills than to share your knowledge of JQuery, Angular, React, or Node?

Free Code Camp Orange County is a great way to get started with web development, level up, and connect with new friends in the OC community.

## Goals
* Projects to collaborate on : TBA
* Goals: Let's get one commit a day
* Download: [TeamViewer11](http://teamviewer.com/en/), [Git](https://git-scm.com/downloads)

## Getting Started with TeamViewer
Normally each week we use TeamViewer 11 to solve FreeCodeCamp's bonfires together. We discuss it and go through it step-by-step, and look for different ways to solve the same problem. 


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
![Fork](http://i.imgur.com/FpYsjMK.png)

To contribute to this repository, you must first fork it. Click the 'fork' button at the top right of this page. This will create you own version of the repository in your GitHub account. Navigate to that page and copy the url in this box.



### Clone to your local machine
![Copy](http://i.imgur.com/5k665GW.png)

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
What this does is push the 'master' branch to the 'origin' remote, in which case should only be ours. See more below on remotes. What has this change done? If everything was done correctly, our forked repository should have "my commit" in the commit history. How do we merge our changes into the main FreeCodeCampOC folder? We can do so by initiating a pull request (Do this on your repo that you have forked).

![Pull request](http://i.imgur.com/ZKndI69.png)


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
