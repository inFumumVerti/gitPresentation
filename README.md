# gitPresentation



My intention of this presentation / introduction was to get a small taste of the possibilities git (and github) so you can use it in your own project. It can often be a huge help when working as a team (or even alone) on a coding project. In the next paragraphs I will recap the most imoortant points I introduced during my presentation: 
## How does Git work
To understand git in the first place you need to understand the "behind the scenes" of git. To simplify the system, have a look at the following graph:

![Stages of git](https://user-images.githubusercontent.com/59310692/140617140-f79f913e-10c5-4e24-92b3-8fec442b196d.png)

It shows the four theoretical stages of git and how they relate to each other. Here's a quick info about each stage:

*Unstaged*: Shows files that have not yet been registred (added) to the git repository and therefore aren't "known" by git.

*Unmodified*: Will include files that have not been altered since the last commit of the current branch.

*Modified*: Shows the files that have been modified in some way since the last commit of the current branch. Deletion is also a modification.

*Staged*: Staged files are files which are ready to be committed into the repository, so they have not been modified since the last 'git add' command. After committing the files are under the 'unmodified' category again.


In reality though, these stages do not exist, but are a concept to make git easier understandable. The real structure consists of three parts, the so-called 'three trees' of git:

![Three trees of git](https://user-images.githubusercontent.com/59310692/140617658-2718b2f4-69b1-4ee9-a8da-ac4ea62d457c.png)



## Git commands

Next up, let's have a look at the basic commands everyone should know to get a simple git workflow going:

*clone*: The first command for many will be the 'git clone' command. It will copy the repository from a given remote repository and immediately create the .git folder, which manages many of the required back-end tasks git accomplishes.

*add*: This command is a very versatile way of sorting the files you do and do not want to commit. Just use 'git add <filename>' to add single files to your next commit. If you want to add all changes in one command, use 'git add .'
  
*commit*: The essence of git consists in the regular update of small chunks of your program. It enables you to have work as a team, make changes faster or just revert an error you accidentally pushed.
  
*checkout*: The checkout command is like three commands in one. You can change (and create) branches, roll back to a previous commit, delete commits or restore files. With all those options it can be hard to get the hang of this powerful command. So here are all the cases:
  
**git checkout < branchname>** will switch to the specified branch.
  
**git checkout < filename>** will restore the file to your working directory. This only works if you haven't committed since deleting the file(s).
  
**git checkout < commit-id>** enables you to roll back to said commit in you current branch. Be careful when using this command, as it creates a "detached HEAD", which can destroy every commit after.
 
  
And lastly,
  
*merge*: The merge command is a great way to combine the progress you made on two different branches into one. It will not alter any of the previous commits in either branch. To visualize this, look at the following:
  
  ![merge](https://user-images.githubusercontent.com/59310692/140618462-8ec7796b-92a0-4b30-b918-e2aa90b096d9.png)
  
  As you can see, a new commit based on both of the merging commits will be created on the branch you selected. This can ofcourse also cause issues. If there are files, which have been edited on both branches, it will cause "merge issues". These can be resolved by deciding which branch can keep it's changes. Oftentimes the IDE you use has a good visual way of doing this taks.
  
 
  
  
  So that is the basic introduction into git. If you have any more questions, go ahead and write me via Discord @Fume#9952
  
  Thank you for reading!
  Linus
