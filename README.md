# Billing-app


## Project description
App to help users take full control of their monthly credit card's expenditures

## Setup local environment

### Clone

If you clone normally and forgot to brought submodules:

    $ git submodule update --init --recursive

If you are cloning the repo for the first time

    $ git clone --recurse-submodules https://github.com/Stefafrontani/billing-app

## Branch Naming

### Configuration

[ project-name ] __ configuration __ [ configuration-description-here ]

### Feature

New 

[ project-name ] __ feature--new __ [ feature-description-here ]

Update

[ project-name ] __ feature--update __ [ feature-description-here ]

### Fix
[ project-name ] __ fix __ [ fix-description-here ]

## Managing submodules

### Add submodule

_./billing-app_
    $ git submodule add [repositoryURL](http://github.com/stefafrontani/billing-app-web)

### Track specific branch from submodule
Follow these steps:

1- Set the branch you want to track:
    
    $ git config -f .gitmodules submodule.billing-app-web.branch develop
    
1.1- Create a branch for the work to be done (not neccesary)

2- Update the submodules of the root repository:

    $ git submodule update --init --recursive --remote

3- Staged the changes:

    $ git add .

4- Commit the changes:

    $ git commit -m ""

5- Push the changes



### Make change to submodule
Follow these steps:

1- Go to submodule:

    $ cd path/to/submodule

2- Make the changes as one would do in any repository

3- Stage changes:

    $ git add .

4- Commit changes:

    $ git commit -m "commit message"

5- Push changes

6- Merge

7- Go to root repository _billing-app_:

    $ cd path/to/root

8- Stage changes:

    $ git add . 

9- Commit changes:

    $ git commit -m "commit message"

10- Push changes