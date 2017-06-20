# GettinGit Tutorial

---

# Some Essential Git Concepts
### To create a new git repository
`$ git init`

*This CLI command creates a new local (on your machine) repository.*

### Repo Status
`$ git status`

*This checks the status of the current repository & shows what files have changed.*

`$ git diff`

*Shows differences/contrasts between the working tree and the latest commit.*

### Repo History
`$ git log`

*Shows all the commits on the current branch. Beginning with the most recent commit.*

`$ git log --oneline --decorate --color --graph --all`

*Illustrates the **full tree history** with a commit graph. This may be easier to read than a `$ git log`*

### Stage files to commit
`$ git add <yourFilename>`

*Add a file and its changes to the staging area.*

`$ git add -A`

*Add all files and changes to the staging area.*

### Commit changes in staged files
`$ git commit -m "<your commit message>"`

*commit staged changes (the `-m` flag will add your commit message inline).*

### Branching off your master branch
`$ git branch <your new branch name>`

*this creates a new branch*

`$ git branch`

*list all branches*

`$ git checkout <your branch name>`

*this switches to a different branch*

### Merging your branches

`$ git merge <your branch name>`

*merge target branch into  current branch.  You will need to checkout your master branch (or desired branch) before running this command.  This command merges the identified branch into the branch you are currently in.*

---

# How to initialize a git repository
**Step One**

*Make a directory*

`$ mkdir <dir name>`

**Step Two**

*Move into the repository*

`$ cd <dir name>`

**Step Three**

*Initalize a git repository*

`$ git init`

---

# Some basic git workflow
*1. **Start** by doing a little bit of work/coding*

*2. **Next** take a second to review your changes you've made*

`$ git status`

*3. **Next** add files to the staging area. (Use `$ git add -A` to add all files and changes.)*

`$ git add <your filename>`

*4. **Next** review what you're about to commit*

`$ git status`

*5. **Finally** commit the changes in the staging area with a message.*

`$ git commit -m "<message>"`

**Note:** You would normally `$ git push` as the next step, however at this point in the walkthrough we haven't added the gitHub repo bindings

---

# Creating/Managing your local repo
### This exercise will reside on your device and not add to a gitHub repo
1. Let's create a new directory in the terminal with the name of your **favorite movie**. (Make sure you `cd` into that directory)
2. Next initialize a local git repository.  (See notes above)
3. Next create a new html file and call it `index.html`
4. Let's check the status of your local repo. Confirm that your new file exists and has not yet been added to your local repo.  (See notes above)
5. Let's add index.html to your staging area.  (See notes above)
6. Let's commit index.html to your local repo with the message "created initial homepage". (See notes above)
7. Next open the file in Sublime and set up your html doc structure. (head, body, title, etc.)
8. Let's check the status of your local repo to view your changes.  (See notes above)
9. Let's add your changes to the staging area.  (See notes above)
10. Next check the status and confirm that your changes have been added to the staging area. (See notes above)
11. Now commit the changes to your local repo with the message "initial html doc structure".  (See notes above)
12. Go ahead and repeat steps 7-11, but add a header to your page this time. Commit these changes with the message "adding index.html header".
13. Now repeat steps 7-11, adding an image of the movie poster. Think about what your commit message should be.
14. Repeat steps 7-11 one more time, add three trivia facts about the movie in an ordered list.
15. Finally run the git log command (`git log --oneline --graph --decorate --all`) to see your local commit history. You should see 5 commits. (See notes above)

---

# Working with a remote repository (gitHub)

`$ git clone <repo path or URL>`

*This clones a repository into a new directory on your local machine*

`$ git remote`

*This lists the remotes for the current repo*

`$ git remote add <remote name> <remote path or URL>`

*This adds a remote to your repo.  A <remote name> example is origin*

`$ git pull <remote name> <branch name>`

*This pulls down any change from a remote and meshes them into your repo. Under the hood it fulfills `git fetch` and then `git merge` commands*

`$ git push <remote name> <branch name>`

*This sends your local project changes to the remote to be merged*

---

# Creating/Managing the Remote Repository (gitHub)
1. In your browser log into your gitHub account
2. Create a repo on gitHub with the name of **gitItGotIt**, don't initialize README.

![NewRepo](../assets/newRepo.png "New Repo Example")

3. Copy the repo URL
4. In the **terminal** add the gitHub repo remote for your local repo.  Name the gitHub repo `origin`
1. In terminal push local commits up to gitHub.
1. Go back to the gitHub repo (in your browser) and confirm that your commits were pushed... Congrats! You've pushed to gitHub! Now your code is visible to the world.
1. In your text editor, add few more interesting facts about your food to the `index.html` page.
1. Check your repo's status, add, then commit the changes with the message "added more food facts".
1. Push your changes up to gitHub. Confirm that the latest commit is there by looking at the commit history on gitHub.
1. In your text editor, add another image of your animal.
1. Check the status of your repo, add, then commit the changes locally.
1. Push the changes up to gitHub.
1. Make a change to the index file using gitHub's web interface and commit the change.
1. Pull down the latest change to your local repo. Congrats! You've now pushed and pulled changes to and from gitHub!

---

# Collaborating with gitHub
### Setup
1. Partner with 2 of your classmates to make a team of 3.
2. Decide who will be partner #1, #2, and #3.

### First
Everyone:

1. Move out of your movie directory and create a new directory called `<your first name>-ThunderCats`.  
2. Move into the new directory and initialize a git repo.
3. Create a new file `ThunderCats.txt`
4. Add the file to be tracked and commit with the message 'created ThunderCats file'.
5. Open the .txt file in your text editor and write the first 3 words that pop in your head.
6. Add, then commit your changes with the message "first 3 words by [your first name]"
7. On gitHub, create a repo called `<your first name>-ThunderCats`.
8. Add the new gitHub repo as a remote called `origin`.
9. Push your local commits up to gitHub.
10. Confirm that your commits are now on gitHub.

Make sure your teammates have caught up before moving on.

### Next Steps
1. Partner #1, go to partner #2's <first name>-ThunderCats gitHub repo and **fork** it. Partner #2, do this to partner #3's repo. Partner #3, do it to Partner #1's repo.
2. Clone the new forked repo (the url should have your username in it) to your computer.
3. Open your partner's ThunderCats.txt file and write add on a new line 3 colors.
4. Add, then commit the change to your local repo.
5. Push the change up to gitHub. Your change should now be reflected in your forked repo.
6. Click the green pull-request button. Review the changes. Click "Create Pull Request".
7. Give your pull request a title and (optional) comment. Click "Create Pull Request" to submit a pull-request to you partner.

Congrats! You've submitted your first pull-request!

Make sure your teammates have caught up before moving on.

### After That
1. Go to your <first name>-ThunderCats gitHub repo. You should see a pending pull-request from your partner. Review the pull-request and accept it if it looks good to you.

Congrats! You've accepted your first pull-request!

Make sure your teammates have caught up before moving on.

### Finally
1. Repeat the steps in Part 2 and Part 3, but this time on your other partner's repo. Instead of writing the 2nd line of the ThunderCats.txt, you should be writing the 3rd and final line of 3 favorite animals.
2. When finished, all three partners should a complete ThunderCats.txt, authored with two collaborators.

---

# Advanced Git
**Aliases** - Make git commands easier and faster to type with command line shortcuts. For more: http://git-scm.com/book/en/v2/Git-Basics-Git-Aliases  

**Rebasing** - Another way to merge that keeps your git history cleaner and more streamlined. For more: http://git-scm.com/book/en/v2/Git-Branching-Rebasing

---

# Additional Resources
Pro Git (free e-book) - http://git-scm.com/book  
Try git - https://try.github.io  
Github Training Videos - https://www.youtube.com/user/GitHubGuides  
Git for Ages 4 and Up (Video) - https://www.youtube.com/watch?v=1ffBJ4sVUb4  
A Practical Git Introduction - http://mrchlblng.me/2014/09/practical-git-introduction/  
Git Branching Game - http://pcottle.github.io/learnGitBranching/  
Github Guides - https://guides.github.com/
