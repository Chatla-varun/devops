# Git Commands Documentation

## Initializing a Git Repository

To initialize a directory as a Git repository:

```bash
git init
```

## Adding Files to Staging Area

To add files to the staging area before committing:

```bash
git add .              # Add all files to staging area
git add filename      # Add specific file to staging area
```

## Committing Changes

To commit staged changes with a message:

```bash
git commit -m "commit message"
```

## Viewing Staged Files

To view files currently staged for the next commit:

```bash
git ls-files
```

## Viewing Last Commit Changes

To see the changes made in the last commit:

```bash
git show
```

## Viewing Commit History

To view the commit history:

```bash
git log
git log --oneline
```

## Pushing Changes to Remote Repository

To push committed changes to a remote repository:

```bash
git push
```

## Pulling Changes from Remote Repository

To fetch and merge changes from a remote repository:

Pull the latest changes: Use the git pull command to fetch the latest changes from the remote repository and merge them into your local branch. If you're working on the main branch (or another branch where you want to pull changes), simply execute:
```bash
git pull
```

If you're working on a specific branch and want to pull changes from a different branch (for example, pulling changes from the main branch into your current branch), you can specify the remote branch:
```bash
git pull origin main
```

## Configuring User Email and Name

To configure user email and name globally:

```bash
git config --global user.email "email@example.com"
git config --global user.name "Your Name"
```

## Checking Remote Repository

To view configured remote repositories:

```bash
git remote -v
```

## Setting Upstream Branch

To set the upstream branch for the current branch:

```bash
git push --set-upstream origin master
```

## Adding Remote Repository

To add a remote repository:

```bash
git remote add origin remote_link
```

## Renaming Branch

To rename the current branch:

```bash
git branch -M master (or main)
```

## Pushing to Remote Repository with Set Upstream

To push the current branch and set the upstream:

```bash
git push -u origin master (or main)
```

## Changing Remote Repository url in linux(https with ssh)

To change the remote repository url:

```bash
git remote set-url origin ssh_url
```
## Generating ssh keys

To generate sshkey( public and private):

```bash
ssh-keygen
```
