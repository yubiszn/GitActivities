# Git Activity 2 - Work as a Team member #
In this second activity, you'll work like you are a member of the team.  This activity will give you a good overview of how you can work with the repository while minimizing your team conflicts.

### Step 1: Complete activity 1 ###
If you have not completed activity 1, you should do that prior to this activity.

1.  Use your `forked` version of the repo to complete the activity.

## Task 2: Checkout a new branch ##
Whenever you start on a new ticket, before you begin any work, you should make sure to get the latest version of the code, then checkout a branch.

In this task, you will run commands to make sure that you have the latest code and that you can do your work in the safest way possible.

1. Get the latest version of the code

    Even though you likely just cloned this repository, it's a good habit to make sure that you have the latest version of the code before checking out a new branch.

    Make sure you have cloned the repo and that your GIT tool is on the master branch.  If you are not currently on the master branch, you can move to the master branch with the command: 

    ```
    git checkout master
    ```  

    Once you are certain you are on the master branch, get the latest code using a fetch and a pull.  You can run them individually, or all at once.  To run them individually, use the following commands:  

    ```  
    git fetch
    git pull
    ```  

    If you would like to run the commands at the same time, you can use the following command: 

    ```  
    git fetch && git pull
    ```  

    Additionally, when branches have been deleted from the remote you can make sure to update your local references with the command: 

    ```
    git fetch --prune && git pull
    ```  
    Running this command will always make sure you get the latest version of the master branch and will let your local references know which branches have been deleted.

    ![Running the git fetch --prune && git pull command](images/Activity2/Image0201.png)


2. Create your new branch  

    With the latest version of the code, it's time to create your new branch.  Hopefully you have a new ticket that you are working on.  With a way to make a unique branch name, follow a pattern that makes sense to your team.  For this example, assume you have a ticket number 54321 and that it is for 'learning git'.  Create a new branch that includes the number, the simple summary, and your name.  For example:

    ```
    git checkout -b 54321-learning-git-brian
    ```

    In the event that the branch already exists, use your initials or your git username to ensure uniqueness.

    ![Checking out a new branch](images/Activity2/Image0202.png)

3. Add a file

    In the folder `TeamMemberFiles` add a new file with your favorite quote, similar to this: 

    ```
    touch myFavoriteQuote.txt
    ```

    ![Creating the new file](images/Activity2/Image0203.png)

    Then open the file for editing in your favorite text editor, and add the following information to the text file.

    * Your Favorite Quote
    * Who said it (yes, it can be from a movie)
    * What is your preferred tech stack (Java/Microsoft/MySql/Sql/Postgres/Vue/Angular/React/HTML/PHP)

    ![The new file is created](images/Activity2/Image0204.png)

    Save and close the file. **NOTE** Do not put personal information in the text of the file. Thanks!

4. Commit your changes

    To commit your changes, first you must stage your changes.  To do this, you would begin by running a command to stage the file changes

    ```
    git add .
    ```  

    Instead of the '.' you could explicitly name the file, but the '.' will include all of your changes.

    Next, commit the changes with the command:

    ```
    git commit -m "<YourName>'s submission for Activity 2"
    ```  
    ![Changes are staged and committed](images/Activity2/Image0205.png)

    Once the changes are committed, push the changes.

5. Push your changes

    Since you've never pushed this new branch, you should run the command

    ```
    git push -u origin <your-branch-name>
    ```
    ![The branch is pushed to remote](images/Activity2/Image0206.png)

    This will push your changes to the remote repository.

6. Create a pull request.

    At GitHub, create a pull request for your changes and tag your instructor as a reviewer on the pull request.

    There are two ways to create a PR.  If you can see your branch has just made changes, you can easily click on the button to create a new PR.  If you can't see your branch having changes, then click on the branches tab. 

    ![Find a way to create the pull request](images/Activity2/Image0207.png)

    If you clicked on branches, find your branch and create a new PR from this screen

    ![If you clicked on branches, find your branch to create the pull request](images/Activity2/Image0208.png)

    After clicking to create the pull request, fill out the comments and assign your instructor and yourself to the PR.  Then hit the final "Create" button

    ![Filling out the details and creating the pull request](images/Activity2/Image0209.png)

    You can see the PR is ready for review at any time.  The person assigned to review should review it and perform the merge.

    ![Reviewing the pull request](images/Activity2/Image0210.png)
    
This will complete your GIT activity.  In this activity, you learned how to work with a branch and create a pull request so that you can ensure your changes can be merged into the repository without creating a conflict.  
