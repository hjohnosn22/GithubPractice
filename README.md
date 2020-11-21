# GithubPractice
Q1 - What does clone set the variable origin to represent?
It sets the variable origin to represent main.

Q2 - What does the command git push --set-upstream origin master do? What does remote tracking mean in this context?
It sets the main branch as the upstream branch (--set-upstream is the same as -u) and pushes any edits to that branch. Remote tracking allows the git on one's PC (in terminal) to process what branch the user is on remotely (even if the user at the moment does not have access to the repo) and gives the user the ability to connect to the repo and upload any changes to the appropriate branch when needed.

Q3 - Explain and illustrate what's happening in the commit tree when this command (git pull origin master) executes.
This command pulls all of the edits from person A's commit to the master branch onto person B's computer. That way they have person A's code while working on the new branch. If person B pushes, their push will not contain person A's edits.

Q4 - Are your commits overwritten by the remote master?


Q5 - Is this a merge or a rebase?


Q6 - Person B: checkout the local master branch. Is it updated as well, or still behind remote master?
It is behind.

Q7 - Run git branch. Did your local copy of your branch delete when Person A deleted the remote branch?
Yes.

Q8 - Use git log --graph --all to view the branching structure and copy and paste the result into the README.md formatted as a code segment (see markdown cheatsheet).


Results of git log --graph --all (some of it, it was very very long)
