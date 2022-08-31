# Steps to follow 📜

## 1. Fork it 🍴
You can get your own fork (copy) of [IntelliMaps](https://github.com/Verisimilitude11/IntelliMaps) by using the `Fork` button at the top right of this page.

![Fork Button](https://github-images.s3.amazonaws.com/help/bootcamp/Bootcamp-Fork.png)

## 2. Clone it 👥
You must move to your fork of the repository and clone (download) it to your local machine using

`$ git clone https://github.com/Your_Username/IntelliMaps.git`

This creates a local copy of the repository on your machine.

After cloning the `IntelliMaps` repository on Github, use the change directory command on Linux and Mac to go to that folder.

```python
# This will change directory to a folder IntelliMaps                                                                   
$ cd IntelliMaps
```
Move to this folder for all other commands.

Let us now add a reference to the original 'IntelliMaps' repository using:

`$ git remote add upstream https://github.com/Verisimilitude11/IntelliMaps.git` 

This adds a new remote named **_upstream_**.

Examine the modifications using:
```git
 $ git remote -v
 origin https://github.com/Your_Username/IntelliMaps.git (fetch)                                                      
 origin https://github.com/Your_Username/IntelliMaps.git (push)                                                        
 upstream https://github.com/Verisimilitude11/IntelliMaps.git (fetch)                                                     
 upstream https://github.com/Verisimilitude11/IntelliMaps.git (push)
 ```

## 3. Sync with the Remote 🔄
Remember to keep your local repository up to date with the remote repository.
```python
# Fetch all remote repositories and delete any deleted remote branches
$ git fetch --all --prune
# Switch to main branch
$ git checkout main
# Reset local main branch to match upstream repository's main branch
$ git reset --hard upstream/main
# Push changes to your forked IntelliMaps repo
$ git push origin main
```

## 4. Create a new branch
Whenever you want to make a contribution,  use the following command to establish a new branch and keep your `main` branch uncluttered (i.e. synced with remote branch).

```python
# It will create a new branch <branchname> with name and switch to branch <branchname>
$ git checkout -b <branchname>
```
 
 To switch to desired branch
```python
# To switch from one folder to other
$ git checkout <branchname>
```

To add the changes to the branch. Use
```python
# To add all files to branch
$ git add .
```
Type in a message relevant for the code reveiwer using 
```python
# This message get associated with all files you have changed
$ git commit -m "relevant message"
```

Now, Push your awesome work to your remote repository using
```python
# To push your work to your remote repository
$ git push -u origin <branchname>
```

Finally, in your browser, navigate to your repository and click `Contribute` amd then `Open Pull Request`. There, please provide a title and description, with brevity, that describe your much-appreciated effort.