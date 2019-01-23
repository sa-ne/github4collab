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
- Clone it to your system
- Make a change by adding your GitHub account name to the list of people that have reviewed this
- Start tracking your changes with git add
- Commit your changes with git commit
- Push your changes to your repository with git push
- Send a pull request to this repository so your change gets included
- Pull these changes into your repository so you have the complete list of all reviewers

## Reviewers
- rhmjs
- marktonneson 2019-01-23
