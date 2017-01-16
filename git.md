##Install

check if you have git installed already

```bash
git --version
```

If not, download [git](https://git-scm.com/downloads).

Download [GitKraken](https://www.gitkraken.com/download).

git is an open source protocol.  gitkraken is a freemium git client that I like to use.  needless to say, use the free version.


##Quick git primer

git is a protocol for keeping track of the history of a directory. it has tools for managing that history and resolving conflicting edits to that history.

Different companies use different "workflows" for managing a git repository.  The most straightforward is:


```bash
git clone

git pull

//... then edit some files, edit files, edit files

git add -A

git commit -m "some message describing your changes"

git push

// repeat starting at git pull
```

Throughout, always use `git status` to check the status of your repository.  Use it frequently, I use it in between every other command I do to double check where things stand.

The flow, again, annotated:

```bash
// this only has to be done once per repository, this 'clones' a remote repository to your local machine.
git clone

// this pulls the latest state of the remote repository down to your local machine.  Try to only do this if your local directory is "clean", ie. free of your own changes.  If not, you may have to merge.  This is something you will need to learn to do eventually but not at first.
git pull

// edit files, edit files, edit files

// this "stages" the changes you just made. when you run a "commit" command, it commits only those changes that have been "staged" for commit.  'git add' is the command which does the staging.  the -A option indicates "all" changes should be staged.  if you only want to stage a few changes, mention those specific files in place of the -A
git add -A

// this "commits" the outstanding changes you have staged.  Pretty straightforward.  You've now created a record of your changes along with the message you've added.
git commit -m "some message describing your changes"

// this uploads the state of your local branch (only that which has been committed) to the remote branch (in our case, the branch stored on Github)
git push

// repeat starting at git pull
```

Note that all of these commands can be run from the GitKraken UI.  Better to familiarize yourself with them on the command line though.  

There is a world of git commands that I haven't touched on here.  Important topics if you come across them include "branches" and "merging".  More complex commands can be run through GitKraken.

There's nothing magic about git.  All the information git stores is stored in a directory at the top level of your repository named `.git`.  What makes your otherwise normal directory a "git repository" is simply the existence of that folder.