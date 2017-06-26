# Git/GitHub Crib Sheet

## Git Repos

Git is version control that allows us to make and track revisions within a directory over time.

**Note:** Make sure you exclude the angle brackets from your commands. These brackets are there to signal you when a unique input is required. 

1) Initiate a directory to be a git *repository*

```
git init
```

2) Edit - create - delete files within the directory
3) Indicate which files you would like included in the next revision

```
git add <filename>
```

4) Commit a revision to the repository's history, writing a message to describe the revision

```
git commit -m "<commit message>"
```

## GitHub Repos

GitHub is a place online where we can store our git repositories.

1) Create a new *GitHub* repository

```
https://github.com/new
```

2) In your local git repo, add a *remote* (which is simply an address) of the GitHub repo

```
git remote add <remote name> <remote url>
```

3) Push your commited work to the *remote* address

```
git push <remote name>
```

## Cloning GitHub Repos

GitHub allows us to share repos with others.

1) Find a repo you want to work on
2) Get the remote url from GitHub
3) Clone the repo to your local machine

```
git clone <remote name>
```

## Forking GitHub Repos

GitHub allows us to make our own copies of existing repos.

1) Find a repo you want your own copy of
2) Fork the repo in GitHub
3) Get the remote url from GitHub
4) Clone the repo to your local machine
