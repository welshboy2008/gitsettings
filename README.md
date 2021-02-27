Git Prompt Settings
===================

This is my git settings stuff. It's stuff I've cobbled together over the years of using git.


## Usage

Clone to repo somehwere, and add the following to your .bash_profile or .bashrc

```
source ~/path_to_files/colours.sh
source ~/path_to_files/git-prompt.sh
source ~/path_to_files/git-completion.sh
```

This will give you a git prompt that looks something like this:

```
emyr@localhost ~/development/someproject (master)*$
```

Where the branch name is on display, and the * tells you if the branch is clean or dirty (i.e. has modifications made to it.)

There's also an alternative to git log in this repo as well, and to use that, run:

```
git config --global -e
```

And add the following to the config

```
[alias]
    lg = log --graph --oneline --all --decorate --color
```

And this will give you a log line that looks like this:

```
* b603850 (HEAD -> master, origin/master) Added basic end point code, and some basic routes (empty). Also updated the config file and the Readme
* 49f1888 Added scripts dir, and an empty script
* be6ab1f fixed readme
* 0a819f9 Added readme
* c4c0c8c Altered git ignore.
* b6af129 First commit of code, built directory structure.
```

And as you branch, you'll get to see branch lines and so on.
