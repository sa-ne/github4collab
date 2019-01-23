# Github Collaboration

## Introduction
This document will introduce the basics of git, GitHub, and Markdown, for purposes of creating a common set of tools and practices to facilitate collaboration on demos, educational material, PoCs, or software projects.
While this document will provide a very basic introduction, these basics can easily be expanded to more advanced uses of git and GitHub, as well as use of other markup languages.

## Prerequisites
- Create a github account
  - If you made it this far, you probably already have an account
  - If not, go here --> https://github.com/join?source=header-home
- Install git on your local Linux system
  - ```yum install git```
- Choose your favorite text editor
  - Atom is a good, multi-platform choice, with git integration
  - https://atom.io/

## Tutorial
- Setup 2-factor authentication
  - Under Settings, Security
- Setup your SSH public key in GitHub
  - Under Settings, SSH and GPG keys
  - Create a new key and copy your **public** key
  - ```cat ~/.ssh/id_rsa.pub```
- Fork this repository in GitHub to your account
  - Click Fork in the upper RH portion of this page
  - Select your account to fork into
- Clone it to your system
  - In your account, under the (now forked) github4collab repository
  - Click Clone or Download, select SSH, copy SSH URL
  - If you setup SSH correctly, running this on your PC should not prompt for a user/password
  - ```git clone <SSH URL>```
- Make a change by adding your GitHub account name to the list of people that have reviewed this
  - Open README.md in your favorite text editor, add your name or github account and today's date to the end
- Start tracking your changes with git add
  - You need to make git aware of the changes you just made
  - ```git status``` git is aware of the change but is not tracking the file
  - Add all files from github4collab with ```git add .```
  - Now run git status again and you'll see the changes are being tracked
- Commit your changes with git commit
  - ```git commit -m "My changes"```
  - You are committing changes locally, adding a message of your choosing
- Push your changes to your repository with git push
  - Now send these changes to your GitHub repository (the one forked from sa-ne)
  - To see where you are pushing to: ```git remote -v```
  - ```git push``` Again if you setup SSH keys correctly this should not ask for user/password
  - You should now see your changes in your Github Account/github4collab repository
- Send a pull request to this repository so your change gets included
  - Now let's send these changes to sa-ne so all can see!
- Pull these changes into your repository so you have the complete list of all reviewers

## Reviewers
- rhmjs
- marktonneson 2019-01-23
