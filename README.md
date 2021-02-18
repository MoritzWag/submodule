# Integration of Submodule in Git Repository

## Setup
1. From the main repository run command: 'git submodule add repository'
2. Initialize the submodules: 'git submodule init'
3. Update in order to pull down the files: 'git submodule update'

## Workflow
### Changes to suresort
In case where changes are only made to suresort, everything works as usual.

### Changes to sslts from suresort
If changes need to be done to the sslts module, adhere to the following steps:
1. change into the directory of the submodule: ´cd submodule´
2. create a branch: git checkout -b new_branch
3. make changes
4. create pull request for sslts (the maintainer of sslts has to proceed)
5. change into the directory of the mainmodule
6. create pull requests for suresort (that includes all changes for sslts)

### Pull changes from sslts to suresort
If changes are made to sslts from sslts:
1. change into the directory of the submodule: ´cd submodule´
2. git checkout main/master
3. git pull origin main/master


### Changes that are not accepted