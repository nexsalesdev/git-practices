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

## Common Configuration for projects
* CRLF should be checked for each file during input 

```
git config core.autocrlf input
```

* Set whitespace checks for trailing space and space before tab

```
git config --global core.whitespace trailing-space,space-before-tab
```
