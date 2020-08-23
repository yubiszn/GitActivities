# Git Activity 3: Create and resolve a merge conflict #
In this activity, you need to create and resolve a merge conflict.  You can do this on any of your own repositories.  If you don't have a repository, you should create one that you can work against.

## Task 1: Create the initial commit ##
To begin, create a new branch off of master.  You can name the branch whatever you would like.  Your repository needs to have at least one file you can modify that has already been checked in.  If you don't have this, first create the repository and make sure to add a file you can easily modify.

1. Create a branch with a name something like merge-conflict-activity-one  

    ```
    git checkout -b merge-conflict-activity-1
    ```  

    In the new branch, modify one of the existing files.  Then add and commit the changes.

    ```
    git commit -am "Conflict activity change 1"
    ```  

    Finally, push your changes out to the repository  

    ```
    git push -u origin merge-conflict-activity-1
    ```  

    Create a pull request but do not merge the pull request.

## Task 2: Create the conflict ##
In this second task, you will modify the same file as in task 1 on a different branch.  This will simulate two team members working on the same file at the same time.

1. Checkout master, then checkout a new branch.

    This activity will reset the file to its original state, and that is to be expected.

    ```  
    git checkout master
    git checkout -b merge-conflict-activity-2
    ```  

2. On the new branch, change the file

    Using the same file you modified on the first activity, create another change that will obviously conflict with the original change.  Save the file, then add and commit your change.

    ```
    git commit -am "conflicting change for demonstration"
    ```  

    Push your change 

    ```
    git push -u origin merge-conflict-activity-2
    ```

    Create the pull request to merge the second change.

## Task 3: Merge the conflict ##
In this task you will merge the pull request and then see the conflict in the original pull request.

1. Merge the pull request for the second change into master.

2. Delete the branch.

3. Update your local repository.

    On your machine, run the command to get back to master.

    ```
    git checkout master
    ```

    Then run the command to fetch and pull

    ```
    git fetch --prune && git pull
    ```

    This will bring the changes you just merged down to your local machine.

## Task 4: Resolve the conflict on the original branch ##
To complete the activity, you need to update your local branch to resolve the merge conflicts, and then you can push your changes out to the remote to fix the merge conflict.

1. Update your local branch

    Begin by checking out the first branch again.  This is the branch that contains your changes with a conflict created by the other merge operation.

    ```
    git checkout merge-conflict-activity-1
    ```

    Next, you either need to merge master or you can rebase.  This activity will merge.

    ```
    git merge origin\master
    ```

    This will merge your commit(s) with the current master.  You will have to resolve any conflicts.  With just one commit this will be trivial.

    Once you have resolved all of the conflicts, commit the changes with a commit message.

    Finally, push your merged changes to remote.

    ```
    git push 
    ```

2. Review the pull request

    Now that you merged the updated master, and pushed to remote, the pull request should no longer show any conflicts.  Merge the pull request to complete the activity.

