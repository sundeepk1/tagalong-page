---
title: "Source Code Management Using Git"
date: 2020-10-26T18:01:08+08:00
description: "Learning to use git"
categories:
  - "DevOps"
tags:
  - "DevOps"
  - "Git"
menu: side # Optional, add page to a menu. Options: main, side, footer
# Theme-Defined params
#thumbnail: "img/placeholder.jpg" # Thumbnail image
lead: "Learning to use git" # Lead text
comments: true # Enable Disqus comments for specific page
authorbox: true # Enable authorbox for specific page
pager: true # Enable pager navigation (prev/next) for specific page
toc: true # Enable Table of Contents for specific page
#mathjax: true # Enable MathJax for specific page
sidebar: "right" # Enable sidebar (on the right side) per page
widgets: # Enable sidebar widgets in given order per page
  - "search"
  - "recent"
  - "taglist"
draft: false
---

Source Control Management (SCM)

Source code management or Version control systems (VCS)  tools are used for managing the codebase developed by developers. Thus, enabling the developers to share the code within the team, without overwriting the changes made by the other member. One of the prominent features of SCM tools is that they are very much effective in tracking the file versions.There are two types of VCS, first Centralized VCS, and second Distributed VCS. 

Centralized version control systems, hosts the source code in one central server and serves all the team members, If this central server crashes then all of our source code is lost. Example of CVS is Subversion (svn).clearcase The second type, as the name suggests is distributed, which serves server-client model, Additionally when the client downloads code, it downloads all the historical changes as well. THe details of this process can be learnt once you familiarize yourself with the tool. 

Specifically, as a DevOps engineer you need to learn git and understand how to manage codebase with git. Learning git is important for us a s DevOps engineers because many of the devops tools and processes like Continuous IntegrationéContinous Deployment (CICD) depend on a particular version of files. In this blog Ièd like to help you with your understanding of git. 

#How to install git
I’ve linked a few videos for the installation of git clients on the popular operating systems. This is pretty much straight forward and resources are available on the internet.
 
## Windows 

{{<youtube nbFwejIsHlY>}}


## Linux
In general linux machines have git client installed. 

{{<youtube gdgravCh_Bw>}}


## MacOS 

{{<youtube PSULlxUk744>}}


#Configuring git
We have to configure our git client so that our information can be made available when performing various git operations. Below are the main configurations that would help us to use git effectively. 

##

#Repositories and branches


#Initializing a repo

##Adding files to the repo

##Commiting files to the repo

##Pushing files to a repo

#How git manages the version history

#Cloning a repo
This means that you are downloading the code from the remote repository t o your local machine, in other  words you are creating a copy of the codebase.
Command used is git clone. 

For e.g 

git clone <REPO_URL>



#Creating a branch and switching to branches 


