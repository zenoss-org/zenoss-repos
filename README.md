============
Zenoss Repos
============

This repository serves as a sort of master repository of various repos that people have come across.
Please create [pull request](https://help.github.com/articles/creating-a-pull-request/), if you know some useful Zenoss stuff. 

If you have some problems with these codes, please ask author of the repo or [Zenoss Community](http://www.zenoss.org/) for help.

Clone with recursive option if you want to clone also submodule source codes:

    git clone --recursive https://github.com/zenoss/zenoss-repos.git 

The format for structure should be as follows:

    top-level repo -
        project_name -
            README.md (link to the project)
            git submodule to repo

Please do not put any actual code in here. Please use full meaning name for the project name, e.g. "*Script Alert HipChat (user)*", instead of "*Zenoss Script (user)*".


## Example

Adding a repo:

    mkdir "project_name"
    git submodule add https://github.com/username/project_name "project_name/repo"
    echo "[Link - project name](http://github.com/username/project_name)" > "project_name/README.md"
    git add "project_name"
    git commit -am "project_name"

Real example:

    mkdir "Script-Alert-HipChat-(carsongee)"
    git submodule add https://github.com/carsongee/zenoss-hipchat "Script-Alert-HipChat-(carsongee)/repo"
    echo "[Link - Script Alert HipChat (carsongee)](https://github.com/carsongee/zenoss-hipchat)" > "Script-Alert-HipChat-(carsongee)/README.md"
    git add "Script-Alert-HipChat-(carsongee)"
    git commit -am "Script-Alert-HipChat-(carsongee)"

