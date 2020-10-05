---
title: GIT essentials
subtitle: Chapter 1 - Intro to VCS
tags: [git, 101]
comments: true
date: 2019-12-31T16:04:44+01:00
---

When I started working back in 2008, [version control systems](https://bitbucket.org/product/version-control-software) (VCS) were merely seen as a companion tool for those rainy days in
case any disaster would happen. Well, at least that was what was explained to me, a junior developer lacking any professional notion. 
My first experience was with [Rationale clearcase](https://www.ibm.com/pt-en/marketplace/rational-clearcase), using an ugly and sluggish UI. With it I was presented to the concepts of
_checkin_ and _checkout_. It was somewhat simple.

_Senior developer_: "So, you will be working on a big and old application. You just need to checkout the code and work over it and then checkin".

_me_: " ¯\\_(ツ)_/¯ Checkout -> Develop -> Checkin ? Roger that. And what does that mean?"

_Senior developer_: "So...man, you take the code from that central place where it is protected and no one touches, put it on your machine, work work work,
and then put it back again!"

_me_: "Uhhh, ok. Seems simple." 

...And this was the usual workflow. 

Some short years after, I moved to a new company where was [Subversion](https://subversion.apache.org/) all the way (Subversion is commonly abbreviated to SVN) . 

Again, a centralized system where the remote repository, also called the "_trunk_", was the main source of truth.
You could checkout parts or all of it. And it was cool as it gave you the flexibility of a file system. Directories and files could be created with any desired structure.

But not all was great. Clashes, AKA conflicts, were a factor of constant mess. If you were not a lucky person working solely on a specific repository then your "Kabummm" odds would be pretty high.

One of the main benefits of a VCS is to allow easy collaborative work...but SVN due to its centralized nature, was not our best friend in the neighbourhood.

# Enter GIT

GIT has come as the holy grail of VCS. With its distributed nature, you were able to manage your workspace versions as you would like , having internet 
or lacking it, the system is completely functional. 
Created by Linus Torvald (Linux creator), one of the greatest minds of our Era, demoted central VCS´s (as SVN) in a blink of an eye.

## Its structure and workflow

The system is composed by 2 repositories - Local, running on your machine; Remote, similar as the central systems, you have a snapshot of your local repo, which entails a 
merged version of everyone collaborating around it.
This remote repo is usually and by standard referred to _origin_.

The local repository, thus its content, is composed by 3 states:

1) Working tree, or working directory, where your new or modified files exist.
2) Staging (or Index), residing all files marked for commit.
3) Commit, or truly on the local repository.

![The 3 states](/images/git-essentials/git-states.png)

The local repo states are better understood if seen from 3 to 1. I like to explain a lot of stuff with metaphor's, some are not that good but so let see:

1. Imagine you want to send a bag of potatoes to New York from Chicago. This bag of potatoes what you will fill (fill a new bag or modify an existent) - Working tree.
2. Then you will put the bag on the train carriage thus marking the bag to go on the next ride - Staging it.
3. Lastly, the train will do its trip until it arrives to Chicago - Commit.
 
Easy right?

This is the first article of a set of articles where I wish to explain the key ideas and concepts around _GIT_.

Stick around and see whats coming out of the stove.