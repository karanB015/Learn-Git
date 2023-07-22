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
