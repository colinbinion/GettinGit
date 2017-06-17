# GettinGit

---

# Essential Git
### Create a new git repository
`$ git init` - Create a new, local repository

### Repo Status
`$ git status` - Check the status of your current repository and see which files have changed.

`$ git diff` - See the differences between your working tree and the latest commit.

### Repo History
`$ git log` - Show all commits for the current branch, starting with the newest.

`$ git log --oneline --decorate --color --graph --all` - View the full tree history with an awesome commit graph, use  instead.

### Stage files to commit
`$ git add <filename>` - Add a file and its changes to the staging area.

`$ git add -A` - Add all files and changes to the staging area.

### Commit changes in staged files
`$ git commit -m "<commit message>"` - commit staged changes (the `-m` flag will let you add your commit message inline).

### Branching
`$ git branch <branch name>` - create a new branch

`$ git branch` - list all branches

`$ git checkout <branch name>` - switch to a different branch.

### Merging

`$ git merge <branch name>` - merge target branch into  current branch.

---

# Initializing a Git Repository
1. Make a directory `$ mkdir <dir name>`
2. Move into the repository `$ cd <dir name>`
3. Initalize a git repository `$ git init`

---

# Basic Git Workflow
1. Do some work
2. `$ git status` to review your changes.
3. `$ git add <filename>` to add files to the staging area. (Use `$ git add -A` to add all files and changes.)
4. `$ git status` to see what you're about to commit
5. `$ git commit -m "<message>"` to commit the changes in the staging area with a message.

---

# Create and manage a local repo
1. Create a new directory with the name of your favorite animal. `cd` into that directory.
1. Initialize a git repository.
1. Create a new html file called `index.html`
1. Check the status of your repo to confirm that your new file exists and has not yet been added to your repo.
1. Add the new file to your staging area.
1. Commit the new file to your repo with the message "created homepage"
1. Open the file in your text editor and set up your html document structure (head, body, title).
1. Check the status of your repo to see your changes.
1. Add your changes to the staging area.
1. Check the status to confirm that your changes have been added to the staging area.
1. Commit the changes to your repository with the message "set up html document structure".
1. Repeat steps 7-11, this time adding a header to your page. Commit these changes with the message "added page header".
1. Repeat steps 7-11 two more times, first adding an image of the animal, the second time adding three facts about that animal in an unordered list.
1. Run the fancy git log command (`git log --oneline --graph --decorate --all`) to see your commit history. You should see 5 commits. Congrats! You've completed the first exercise.

---

# Working with a remote repository (Github)

`$ git clone <repo path or URL>` - clone a repository into a new directory.

`$ git remote` - List all remotes for the current repo.

`$ git remote add <remote name> <remote path or URL>` - adds a remote to your repo.

`$ git pull <remote name> <branch name>` - Pull down changes from a remote and integrate them into your repo. Performs `git fetch` and then `git merge`.

`$ git push <remote name> <branch name>` - Send your changes to the remote to be merged.

---

# Create and Manage a Remote Repository
1. Log into your GitHub account
1. Create a repository on GitHub with the name of your favorite food. (Don't initialize a readme). Copy the repo URL to your clipboard.
1. On your command line: Add the github repo as a remote for your local repo. Give the github repo the name `origin`.
1. Push your local commits up to github.
1. Go back to the GitHub repo (in your browser) and confirm that your commits were pushed... Congrats! You've pushed to GitHub! Now your code is visible to the world.
1. In your text editor, add few more interesting facts about your food to the `index.html` page.
1. Check your repo's status, add, then commit the changes with the message "added more food facts".
1. Push your changes up to Github. Confirm that the latest commit is there by looking at the commit history on GitHub.
1. In your text editor, add another image of your animal.
1. Check the status of your repo, add, then commit the changes locally.
1. Push the changes up to GitHub.
1. Make a change to the index file using GitHub's web interface and commit the change.
1. Pull down the latest change to your local repo. Congrats! You've now pushed and pulled changes to and from Github!

---

# Collaborating with Github
### Setup
1. Partner with 2 of your classmates to make a team of 3.
2. Decide who will be partner #1, #2, and #3.

### First
Everyone:

1. Move out of your food directory and create a new directory called `<your first name>-ThunderCats`.  
2. Move into the new directory and initialize a git repo.
3. Create a new file `ThunderCats.txt`
4. Add the file to be tracked and commit with the message 'created ThunderCats file'.
5. Open the .txt file in your text editor and write the first 3 words that pop in your head.
6. Add, then commit your changes with the message "first 3 words by [your first name]"
7. On GitHub, create a repo called `<your first name>-ThunderCats`.
8. Add the new GitHub repo as a remote called `origin`.
9. Push your local commits up to GitHub.
10. Confirm that your commits are now on GitHub.

Make sure your teammates have caught up before moving on.

### Next Steps
1. Partner #1, go to partner #2's <first name>-ThunderCats GitHub repo and **fork** it. Partner #2, do this to partner #3's repo. Partner #3, do it to Partner #1's repo.
2. Clone the new forked repo (the url should have your username in it) to your computer.
3. Open your partner's ThunderCats.txt file and write add on a new line 3 colors.
4. Add, then commit the change to your local repo.
5. Push the change up to GitHub. Your change should now be reflected in your forked repo.
6. Click the green pull-request button. Review the changes. Click "Create Pull Request".
7. Give your pull request a title and (optional) comment. Click "Create Pull Request" to submit a pull-request to you partner.

Congrats! You've submitted your first pull-request!

Make sure your teammates have caught up before moving on.

### After That
1. Go to your <first name>-ThunderCats GitHub repo. You should see a pending pull-request from your partner. Review the pull-request and accept it if it looks good to you.

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
# pizza
