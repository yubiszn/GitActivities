# Git Activity 1 - Forking a repository

This first activity will get you setup to complete the rest of the activities.

If you are struggling with any of the concepts required for this assignment, make sure to review the video course to find out more about how to perform a specific command, or just get more practice and understanding of the topic presented.


### Step 1: Fork this repository ###
To begin, you need to fork the repository.  Any time you are going to work on someone else's project, but want to potentially contribute, the correct way to proceed is to fork the repository.

1. You are already on this repository, so all you have to do is fork it to your own account.

    To begin, make sure you are on the correct repository, find the `Fork` button, and press the button to fork this repository to your own account.

    ![Fork the repository](images/Activity1/Image0101.png)

2. Select the correct account where you want to fork the code.

    For example, select the account you use for the current Organization.

    ![Select Your Account](images/Activity1/Image0102.png)

    While the operation is taking place, a dialog is shown that will give you information about what is happening.

    ![Select Your Account](images/Activity1/Image0103.png)


3. Once the fork operation is completed, you have your own copy of the code.

    Your account name and repo are shown, as well as the account from which you cloned.

    ![Your account details for the forked repo are shown](images/Activity1/Image0104.png)  

    Additionally, you are given information about the commits in your repo compared to the original.

### Step 2: Understand the relationship ##
To complete this activity, you just need to understand the relationship between your account and the base repository.

The base repository is where you forked, and your repository is where you will do the work.

1. Clone your repository.
    
    In order to do work locally, you'll need to clone your new repository.  Use the `Code` button to get the url, and clone the repository to a location you can easily remember and work with in the future.

    ![Your account details for the forked repo are shown](images/Activity1/Image0105.png)  

    Use BASH or any of your favorite GIT clients to clone the repository locally.

    Copy the url, make any directories you need and make sure your command line is on that directory, then run the command:  

    ```
    git clone <your-repo-url>
    ```  

    ![Run the clone command](images/Activity1/Image0106.png)  

    You now have a local copy of your code to work with.

2. Make a quick change to see how all of this works.

    It doesn't matter what you do here, just add a file or modify an existing file, then save it.

    Once the file is saved, make sure you have the changes ready with a git status command: 

    ```  
    git status
    ```  

    ![Check status to see changes pending](images/Activity1/Image0107.png)  

    Then run the command

    ```
    git add .
    ```

    ![Adding files stages them for commit](images/Activity1/Image0108.png) 

    Which will move your change from modified or untracked to staged.  

    >IMPORTANT: Changes will not commit if not staged.

    With the changes staged, run the command:  

    ```  
    git commit -m "My first commit after changes"
    ```  
    ![Run the clone command](images/Activity1/Image0109.png)  

    Finally, push the commit you just created locally to the remote repository:  

    ```
    git push origin master
    ```
    ![Push changes from local to remote](images/Activity1/Image0110.png)  

    In future activiites, you will learn about branching strategies.

3. Open a pull request from your repo to the original.

    In a real project, if you were making modifications, you could request the original person accept your changes from a pull request.

    Opening a pull request now will connect your repository to the main repository in order to let htem accept your changes into the base repository. 

    Your repository should be at least one commit "ahead" of the other repository.  You may also be "behind" meaning others have made changes at that repository.  If others have made changes, you may have a conflict.  You would have to resolve the conflict before your "code" can be merged.

    ![You can see if your code is ahead or behind at any time](images/Activity1/Image0111.png)  

1. Use the link for "Pull Request" to make a new pull request.

    Click the link to start the process.

    ![Begin a pull request](images/Activity1/Image0112.png)

2. With the pull request started, select your repository -> master branch into the base repository master branch.

    You can do a PR from any branch to another.  As you can see, you can also do the PR from one repo to another, as long as they are connected.  

    ![Begin a pull request](images/Activity1/Image0113.png)

    Rest assured that only people who are allowed to do so will be able to merge your PR.  You may have to wait, days, weeks, months, or even years before the repository owner lets your code into the base repo.  

    ![The repo owner will approve or deny your pull request](images/Activity1/Image0114.png)


# Completion Criteria #
At the end of this activity, you should have completed the following:   

*   You have forked the GitActivities Repo.  

*   You cloned the repo locally to your own machine.  

*   You added and committed a change to your local repo.

*   You pushed the local changes to your remote repo.

*   You have opened a PR to the base repository.  Leave this open as part of the week 1/2 requirements.