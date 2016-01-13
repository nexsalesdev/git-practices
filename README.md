# Git Practices at Nexsales

This is a sample project meant as a reference for git configuration for all projects at nexsales.
It sets the guidelines and provides reference for setting up of a new repository for nexsales 
projects.

## Basic Guidelines to follow
* Have a README.md file which provides information about the project. It should also include the 
build status from CI.
* Include a LICENSE.md file which contains the project license.
* Add a .gitignore file which ignores files that should not be checked in to the project. e.g.
  - Compiled Binaries
  - Temporary Files
  - Dependent Projects which can be included using other mechanisms
  - Editor swap files
* Include a .gitmessage file which should be added as a git commit message template.

## Local Git Setup for users
* Ensure Full Name is set for the user

```
git config --global user.name "Foo Bar"
```

* Ensure Email address is set for the user

```
git config --global user.email foo.bar@nexsales.com
```

* Recommended: Set a difftool. Use git difftool to analyze diffs instead of git diff.

```
git config --global diff.tool $EDITOR
```

Recommended: Set a mergetool. Use git mergetool to merge instead of git merge.

```
git config --global merge.tool $EDITOR
```

## Common Configuration for projects
* CRLF should be checked for each file during input 

```
git config core.autocrlf input
```

* Set whitespace checks for trailing space and space before tab

```
git config --global core.whitespace trailing-space,space-before-tab
```
