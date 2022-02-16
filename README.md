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

### before and after most everything I do, I run ```git status``` just to make sure im in the branch that I want and to see if I have any new code that I forgot to push or something. Code that you have that is different from the main branch and hasn't been commited yet will be red when you run ```git status```

---

After you've written some code that you want to push to your branch, you can do a couple of things

1. Run ```git status``` to see what files you've written code to have changed (they'll be red). It might be the case that you don't want to push everything up--maybe you were testing something out in some file in addition to writing code that you want to commit in a differnt file and maybe you don't want to push that testing code.

    Say you wrote something in a file, random.js, and also something you're really working on in coolThing.js. If you want to commit just coolThing.js, you can run:<br>
    ```git add path/to/coolthing.js```<br>
    ```git commit -m "descriptive message about what you're committing"```<br>
    ```git status``` to make sure that the code you want to commit is now [Red].<br>
    ```git push origin your-branch-name```<br>
    
---

OK so now, in a perfect world, your new code has been committed and pushed to github.com and is inside a branch that you created. When you want to merge your branch with the master/main so that your team can pull your new code, go to the project repository on github.com (there are a few ways to do this but I think this is the most straightforward/visual way) and there should be a new pull request that'll look like this (notice the yellow bar that has a green button that reads: "Compare and Pull Request":<br>
<div align='center'>
        [<img src="https://opensource.com/sites/default/files/uploads/compare-and-pull-request-button.png">](https://opensource.com/sites/default/files/uploads/compare-and-pull-request-button.png)
</div>

