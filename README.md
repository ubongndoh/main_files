# main GiftAPad repository. This is the project carried out by members of #team_berlin in the three weeks start.ng pre internship programme. This project was built remotely by each contributor thanks to githubcd main_filescd main_files FOR TEAM MEMBERS... Thank you for coming, please attach screen shot while making a pull request. Also use the main.css to style all your codes. Don't forget to comment on your part

#Username on Slack - @Francis-Xavier
#I created the contact page, edited the about and index page, changed main.css to style.css and created a separate stylesheet called contact.css for contact page located in the css folder.

#slack username: Taofeeq-deru
#I added the donation page and also added the stylesheet for the donation page css folder. Also added font-awesome-4.7.0 which I used in creating the donation page


#Username on Slack - @Francis-Xavier
#I created the project.html page and project.css. Added hr styling to the footers. Updated the team page with my details.

# Contributions

## Fork the repository

go to https://github.com/giftapad/main_files , fork the repository by clicking on the _fork_ button at the top of the page,

![ScreenShot](https://res.cloudinary.com/raphaelnagato/image/upload/v1567259047/gitapad2.png)

## Clone the repository

go to your forked repository on your Github profile and copy the URL to your forked repository, from _clone or download_ button

![ScreenShot](https://res.cloudinary.com/raphaelnagato/image/upload/v1567259048/giftapad_3.png)

then go to your terminal on your computer and type

`git clone "url you just copied"` e.g `git clone https://github.com/your-username/main_files.git` .

## Create a branch

on your terminal, type `cd main_files` , then create a new branch by using `git checkout` command, `git checkout -b <name-of-new-branch>` , e.g `git checkout -b add-raphael`

## Make necessary changes

open the folder on your favourite code editor and navigate to team.html,
![ScreenShot](https://res.cloudinary.com/raphaelnagato/image/upload/v1567259047/giftapad4.png)

add your link to your cloudinary photo (replace, the default link), Add your name and track, then save.

Go to the terminal and enter `git status` command, you should see the unstaged files highlighted in red.

stage the changed file by using the command `git add .` or just `git add team.html`

(using `git status` command again, will show the files changed highlighted in green)

commit the files using `git commit -m 'your-commit-message'` e.g `git commit -m 'add-raphael-profile'`

## Push your changes to github

push your changes to github using `git push` command

i.e `git push origin <your-branch-name>` replacing <your-branch-name> with the name of the branch you created earlier, e.g `git push origin add-raphael`

## Submit changes for review

If you go to your repository on github, you should see compare & pull request button, click on it

![ScreenShot](https://slack-imgs.com/?c=1&o1=ro&url=https%3A%2F%2Fhisham.hm%2Fimg%2Fposts%2Fgithub-comparepr.png)

Now submit the pull request by clicking on _create pull request button_ , remember to add a screenshot of the `team.html` page after your effected changes when opened in browser.

![ScreenShot](https://slack-imgs.com/?c=1&o1=ro&url=https%3A%2F%2Fraw.githubusercontent.com%2FRaphaelNagato%2Ffirst-contributions%2Fmaster%2Fassets%2Fsubmit-pull-request.png)

Soon, your changes will be merged by the team lead _@Ezeko_ or his deputies.

![ScreenShot](https://res.cloudinary.com/raphaelnagato/image/upload/v1567261134/giftapad5.png)

_CONGRATS ON YOUR FIRST CONTRIBUTION!!!_

## What next?

Check for tasks on _#teamberlin_'s workspace, collaboration will follow this standard _fork-clone-create new branch-edit-commit-pullRequest_ workflow.

# Keep forked repository in sync

_After Forking and cloning your repository, you start contributing to the main repository and after a while, you notice that your forked repository and the upstream repository are not in sync anymore, usually noticed when your branch have conflicts with the main branch. This guide will make you get the current version of the upstream repository._

## Add the Upstream

The original repository is mostly called `upstream` . In our case, that would be `https://github.com/giftapad/main_files.git` , `cd` into your forked repository, you should preferably be on the `master` branch. To add `upstream` you use the command;

`git remote add upstream git://github.com/giftapad/main_files.git`

Using the `git remote -v` command after, you should see the following;

![ScreenShot](https://res.cloudinary.com/raphaelnagato/image/upload/v1567518500/clodinary_upstream.png)

if you made any mistakes in the URL when adding the upstream, you could always use `git remote remove upstream` , and repeat the process again .

## Fetch and Merge upstream with forked repository

Now that we have both URLs, we can now use the command `git fetch upstream` to fetch all the changes from the upstream and then we merge the changes using:

`git merge upstream/master master`.

you can do all this with just `git pull` i.e `git pull upstream master`

## Keeping remote origin up to date

After the previous step, if you type the command `git status` , you should get a message like;

![ScreenShot](https://res.cloudinary.com/raphaelnagato/image/upload/v1567519673/behind_giftapad.png)

This is because, you have only updated your local repository, to update your remote repository, that is the one on GitHub,you will have to use `git push` command i.e `git push -u origin master`.

refreshing your remote repository on GitHub should show that your `branch` is even with `giftapad:master`.
