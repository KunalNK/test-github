**Lab01: Git Commands**

1. Create a directory called working\_with\_git and cd into it. >> **mkdir working\_with\_git && cd working\_with\_git**.
1. Once in this directory, initialize a git repository.>> **git init**
1. If you then type git status, you'll be told that there's nothing to commit. >> **git status**.
1. From your working\_with\_git directory, create a file called example.txt >> **touch example.txt**.
1. If you run git status now, you should see that this new file is not tracked yet. >> **git status**
1. To track this file, we can type >> **git add example.txt**, which tells git to add everything that's changed in the current directory to the staging area.
1. Once you have added all the files you would like to the staging area, the next step is to commit with a message.
1. So once you have added, you can then type >> **git commit -m "initial commit"** and you will make your first commit.
1. To see what your commit history looks like, you can type **git log.** To close out of **git log**, you can press **q.**
1. To see your commits in a bit of a cleaner fashion, you can add the **--oneline** flag to the **git log** command. So if you type **git log --oneline** you will see each commit on one line, which may be easier for you to read.


















**Exercise01: Git Commands**

1. Create a folder called **learn\_git**. (Make sure you do this from a folder that isn't a git repository!)
1. cd into the **learn\_git folder**.
1. Create a file called **first.txt**.
1. Initialize an empty git repository.
1. Add **first.txt** to the staging area.
1. Commit with the message **"adding first.txt"**.
1. Check out your commit with git log.
1. Create another file called **second.txt**.
1. Add second.txt to the staging area.
1. Commit with the message **"adding second.txt".**
1. Remove the **first.txt** file.
1. Add this change to the staging area.
1. Commit with the message **"removing first.txt".**
1. Check out your commits using git log.


























**Lab01: Merging**

\1. Create a folder called learn\_branching and cd into it => mkdir learn\_branching && cd learn\_branching.

\2. Initialize a git repository => git init.

\3. Create a file called first.txt => touch first.txt.

\4. Add that file git add ..

\5. Commit that file git commit -m "initial commit".

\6. Create a new branch called feature => git checkout -b feature.

\7. Now that you are on the feature branch, create a file called new.txt => touch new.txt.

\8. Add that file => git add ..

\9. Commit that file => git commit -m "adding new.txt".

\10. Create another file called another.txt => touch another.txt.

\11. Add that file => git add ..

\12. Commit that file => git commit -m "adding another.txt".

\13. Change back to the master branch => git checkout master. Note that this branch has no awareness ofnew.txt or another.txt!

\14. Merge our changes from the feature branch into the master branch => git merge feature

\15. Delete our branch called feature => git branch -D feature

**Exercise 01** 

\1. Create a folder called branch\_time.

\2. cd into that folder.

\3. Initialize an empty git repository.

\4. Create a file called first.txt, then add and commit the file.

\5. Create a new branch called amazing\_feature.

\6. Create a file called best.txt.

\7. Add the file.

\8. Commit the file with the message -m "added best.txt".

\9. Switch back to the master branch.

\10. Merge your changes from the feature branch into master.

\11. Delete the feature branch.

**Lab03: Remote repository on Github**

1. Create a remote repository “demo-github”.
1. Clone the repository on your local machine by typing git clone <repo-url>.
1. **echo "#demo-github" >> README.md** - we are passing some markdown into a file called README.md.
1. **git init** - make sure we have a repository.
1. **git add README.md** - let's add the README.md file to staging area.
1. **git commit -m "first commit"** - add a commit with the message "first commit"
1. **git remote add origin** <<repo-url>> 
1. **git push -u origin master -** Now we can send our code from a local repository to our remote repository.

**Exercise03:** 

1. Create a local repository test-github & initialize it.
1. echo "Hello world" >> test.txt.
1. Add file **git add test.txt**
1. Commit that file **git commit -m "initial commit"**.
1. Create a remote repository **test-github**.
1. git remote add origin <<remote repo url>>
1. Push changes of local repo to remote repo using   **git push origin master**.

