# Jevargass.github.io
Questions from Jeff
1. When should you use Git for a project?
Git is a great method and good to help streamline development for programming projects. It comes with no language requirements nor file structure requirements, leaving it open for the developers to decide how they want to structure their workflow..

2. What kind of files/info should be saved in a Git repository? What types of files/info should not be included in a Git repo?
Git public repositories can contain text files with code, and information that is not sensitive. They should not contain large files and sensitive or personal information, unless you get a private repository. Note, however, that private repositories are still stored on external servers.

3. What are the commands to undo a commit?
$ git commit -m "a bad commit"              
$ git reset HEAD~1     
THEN

$ git add .                                              
$ git commit -c ORIG_HEAD                                   
This way will keep the changes that were bad (the commited file will still be staged), but will no longer be the master while you change your file. If you want to entierly delete the commited file (although theres still ways to get it back after), instead of $ git reset HEAD~1 you can use $ git reset --hard HEAD~1. This will return the file to its state before the state seen in your bad commit.

4. One of your repositories is in a “detached HEAD” state. How do you fix this?
You have a few choices depending on what you want to do. If you want to return to the branch you came from git checkout -(the dash is a shortcut for the last commited branch) or more specifically git checkout [branch name] will do the trick . However, if you made some changes to the file you are now looking at (which is not necessarily the most recent file on your branch, aka the master) which you want to keep, you need to specify that you want to commit this and make a new branch out of it using git checkout -b [name of your new branch].


5. Your boss has no idea what Git is or why you are using it. Explain the pros / cons of using Git for your research project. Explain the pros / cons of hosting your project in a public (or private) repository on Github/Bitbucket/Gitlab/etc.

+My Biology 824 Assignment on Version Control
 +
 +My page: https://Jevargass.github.io/
