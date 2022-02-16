# git-shit

---

Before you do any work, run
```terminal
git pull
```
This will update what you have to match with the master/main branch that is on github. This is how you'll get all the new code your team has pushed. As long as you're making sure that you're only working on code in your own branch, there shouldn't be any issues with merging. If you made a booboo and worked on code in the main/master branch, there's a chance that when you do a ```git pull``` some of your code will be overwritten :cold_sweat:

---

When you want to start working on your own shtuff you'll want to create a new branch or switch to one that you've already created and are working on.

See all branches:
```terminal
git branch
```

See all remote branches (remote meaning branches that everyone on the team has made):
```terminal
git branch -r
```

create a new branch and switch into it:
```terminal
git checkout -b whatever-you-want-to-call-your-branch
```

swich to a branch
```terminal
git checkout whatever-the-branch-name-is
```

### before and after most everything I do, I run ```git status``` just to make sure im in the branch that I want and to see if I have any new code that I forgot to push or something. Code that hasn't been commited will be green when you run ```git status```
