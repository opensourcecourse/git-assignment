# Git assignment

Now we get to practice git! You are encouraged to use git through the command line for this assignment,
but you may use VCS integration with your IDE in the future. If you get stuck, first try typing
something like "How to do X in git" into google before asking for help. You will find solutions to
almost any git question on stackoverflow.

Answers to each task will be input to "answers.md" of this repository. You can edit this directly using
the git web interface by clicking on "answers.md" in a new window, then click the edit button. Make sure
you click on "Create a new branch for this commit and start a pull request." rather than commiting directly
to main. See
[here](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files) for more
details.

# Task 1: Fork, clone (5 points)

Fork the git repo named "git_repo" from the course organization. Make sure to fork all branches by unchecking
the "fork only main branch" checkbox. The repo can be found [here](https://github.com/opensourcecourse/git_repo).

Next, Clone the repository to your local computer. Copy the output of the git status command in answers.md

Hints:

[Github fork documentation](https://docs.github.com/en/get-started/quickstart/fork-a-repo)


# Task 2: Modify, push (5 points)

Add your name as a markdown link with a target to your personal github page to the file "students_who_win.md".
It should look like this:

```
[Derrick Chambers](github.com/d-chambers)
```

Add the changes then commit. Make the commit message read "completed Task 1". Push the changes back 
to your fork. 

Next, paste the commit hash for the commit you just made under task 2 of answers.md. Here is an example commit hash:

b0650b0f1fe6f2b831feb162879ce50da75784be

Hint: remember git log

# Task 3: Git diff (5 points)

First, use `git branch` to see the current *local* branches. Now look at the remote branches with `git branch -a`.
The `-a` tells git to look at all branches, not just the local ones. 

Next, checkout branch_2. This will create a local copy of branch_2. Run `git branch` to verify a new local branch
named branch_2 appears in the list.

Now, use the git diff command to find the differences in *only* the file "myscript.py" between main and branch_2.
Paste the output of the command under task 3 in answers.md. What is the difference in this file? Do you suspect
merging branch_2 and main will cause a conflict? 


# Task 4: Conflict resolution (5 points) 

Next, checkout the main branch again and merge branch_2 into it. Resolve the conflict and commit. Make the commit
message read "merge branch_2 into main" and push the new commit back to your fork. Paste the commit hash in answers.md
under Task 4.

# Task 5: Rebase and squash (5 points)

Next, checkout branch_1 and rebase it to main. Push the changes from branch_1 to your fork.

Hints:
 - Read the output of git rebase *carefully*, it will tell you what to do.
 - When pushing, use the force.
 - [More on rebasing](https://stackoverflow.com/a/11566503/3645626)

Now, squash all commits on branch_1 into a single commit, and push again. Paste the hash of the commit in 
the Task 5 of answers.md

# Task 6: Archeology (bonus, 5 points)

A file called "secret.py" once existed in this repo. Use your git foo to find the commit hash it was created,
deleted, and the comments of the file. Post your answers in Task 6 of answers.md

# Submit PR

Finish editing answers.md. Ping the instructors with a comment that includes @instructors to let them know
you are ready for feedback. Wait. 

# More hints

If things get hopelessly mangled: ![](https://xkcd.com/1597/)
[Local and remote branches](https://stackoverflow.com/a/72156/3645626)

