# How to play Exquisite Git

- ask for help EARLY AND OFTEN
- don't work ahead (even if you definitely know what's next)
- have fun :)


## Game set up

### make new branch

`git checkout main`

`git pull`

for your branch name, use the number that was assigned to you, spelled out **in lowercase** such as "one" or "two"

`git checkout -b {put your branch name here}`

### make changes to your files

create a new file with the same name as your branch

add the first line of a story to the file

**save it!** don't forget to save!!

### stage changes using git add

Use one of these: 

`git add .` adds all files in the current directory (if your `pwd` is the root of the repo, that's **everything**)

`git add -A` adds all tracked and untracked files

`git add {path}` adds files at the specified path (it could be a path to a directory or just a single file)

### commit changes

files have to be added by this point or your commit will be empty

`git commit -m "commit message goes here"`

### push commits

the first time you push to a brand new branch: `git push -u origin <first-name-code>`

The `-u` is short for `--set-upstream`, it creates the relationship between your **brand new branch** and a new linked branch on the remote

## Game play

Once you finish the previous round and you're sure your story is pushed (you can check the web interface if you're not sure) and your moderator says it's time to start the next round, you may proceed.

We will rotate through the numbers. If you started as `two`, your branch is now `three`. If you're the last number in the group, your branch is now `one`. 

### for each round: 

1. `git checkout {branch-name}` replace branch-name with the name of your *new* branch.
1. `git pull` **THIS IS IMPORTANT!!**
1. open the story file
1. write a line that follows the line that's already in the file
1. **delete the line that was already there**! The next person who checks out this branch should *only* see your new line. 
1. `git add .` or `git add -A` or `git add {name of file}`
1. `git status` to make sure your changes appear in green (and nothing else!)
1. `git commit -m "story update"` (or whatever commit message you like)
1. `git push`
    * it's not necessary to use `-u` or `--set-upstream` because this branch already exists on the remote, and already has established the relationship between the local and remote. 
1. **WAIT!!** Don't move on until your facilitator says it's time for the whole group to proceed to the next round.

## Finishing the game

When we finish the final round, it's time to reconstruct our stories by referencing the git history. There are several ways to do this, your facilitator will demonstrate and guide you through this process. 
