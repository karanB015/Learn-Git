# GIT

Free and open source version control system, most widely used.

# Version control: 
    way to track the progress of the program or the code changes.
    So basically we add/save the current program and then we cn proceed further.
    Afterwards, we can trace back all the changes made over time.
    We can go back to previous version or check the bugs.!

    1. Directory -> Folder on the local system.
    2. Repository -> Project or the folder where project is kept.
    3. GitHub -> Wbesite to host the repositories online.

1. Clone: Bring the repo. from the hosted website on the folder on local machine.(GitHub to local)
2. Fetch: 
3. add:
4. Pull: Download the changes from the remote repo to the local machine. (opposite of the push)
5. commit: 
6. Push: 

-> ".git" is the hidden folder which stores all the project versions that we have been committed.
# Steps:
    1. git init -> Just to create a local repository locally in a folder to get ".git"
    2. Create an empty repo online, to basically push our work to.
    3. Either add the repo to a remote list on the machine like:
        git remote add origin <HTTPS-Link>
        git remote -v: To check the list of the available remote repositories.
    4. Or simply we can directly push to a specified repo directly:
        git push https://github.com/karanB015/Learn-Git.git

# git add:
-> Basically .git should track all the files in the directory for the modification or a new creation.
-> git status will show the untracked files to be staged or added, to be further committed. 
-> "(master *+)", the tag shown on the cli when the changes made are not staged or added using "git add <filename>".
-> "(master +)", tag shown on the cli after the changes have been added.  
-> Files/Folders which are not added/staged will not get committed/saved in the local git. 
-> Therefore, we need to use "git add <filename>" to add/stage the modified file/folders, which will be committed later all at once.

# git commit:
-> Now git has added all the changes, which are supposed to be saved locally for the version control.
-> "git commit -m <message>"
-> It will control all the versions locally in the system.
-> Now, its ready top be pushed to the online repository.

# git push: 
-> We need the access token as a password.
-> Login to the github account - profile - settings - Developer setting - Personal access tokens - Generate new tokens()
-> Add a a note and give all the permissions - generate the token.
-> "git push https://github.com/karanB015/Learn-Git.git" 
-> Username: <Username> of the account.
-> Password: <accessToken>

# Branching:
 -> Lets say we create a new branch of our project(feature branch).
 -> The base code will be same but with a we will be updating it with new features.
 -> After the job is done, we will merge it back to the master branch.
 -> "git branch" will show all the available branchbes on the local machine.
 -> "git checkout -b <branch>" it will create and take us to the side branch. (-b is to create the branch).
 -> "git checkout <branch>" to just move to the specified branch.
 -> The moment we push, we create/update the same branch online, untill specified.
 
 Note: whenever we create a branch, its a complete new and separate copy of the base project. 
        Therefore, after that in each branch we can have different content, untill merged
        

# git pull request:
 -> To merge the branches, online.
 -> This way we can review and compare befor merging.
 -> 

 Note: But ofcourse, we merge the branch to lets say master, the local master has no clue about that.
        So, we need to get those changes in local as well, therefore, "git pull" will get all the changes required.

 -> Its a good practise to delete the branch after merged, "git branch -d <branch>".

# git merge:
 -> We in the child branch, "git merge <master>".
 -> We might get merge conflicts, to be solved manually.

# git fork:
 -> To get someone else's repo under our account.
 -> This way we can work with it under our account.
 -> We can merge it with actuall project later.