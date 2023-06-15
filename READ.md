In this ungraded lab you will practice version control by forking a repository, creating a branch and committing a change. Once your changes are staged you will open a pull request with the source repo.
Goal

    Create a pull request from a forked repository.

Objectives

    Fork a repo

    Clone a forked repo locally

    Create a branch

    Add and commit changes

    Push changes

    Open a pull request

Learner Instructions

Step 1: Open the Terminal and authenticate using gh (Github CLI): 

gh auth login

Note: If you receive a message after gh auth login: "You're already logged into github.com. Do you want to re-authenticate?" you can select "No" as you're already authenticated and will not need to complete this step again at this time

Step 2: Create an authentication token in your Github account with specified scopes given in the terminal. Copy it from Github and paste it. Verify authorization was successful.
Verify that authentication was successful. 

Step 3: Visit the class repo

 and click the fork button. A Create a new fork view will appear. Select the dropdown for the owner to the account you want to fork to. Keep the default name and then click on the Create Fork button. 
Click on Fork button

Step 4: After the project has been forked into the account you chose from step 3. Clone the forked repository using the GitHub CLI command. 

Clone the repository. 

gh repo clone <YOUR USERNAME>/<REPOSITORY-NAME> 

Step 5: Move to the repo directory by using cd <REPOSITORY-NAME>

Step 6: Create and checkout a new branch.

git checkout -b my-branch 

Step 7: Open and edit the class.md file

    Add your first name

    Add the name of the certification you are working on

Step 8: Add your changes

git add class.md 

Step 9: Commit your changes with a message using the -m flag

git commit -m 'minor changes'

Step 10: Push your changes to your fork

git push origin my-branch 

Step 11: Visit the class repo and click Pull Requests.

Step 12: Click on New Pull Request.
New pull request button

Step 13: On the compare page click "compare across forks"
Compare across forks link

Step 14: Select the main branch as "base"

Step 15: Select your fork and the committed branch (my-branch) as "fork" and then click on the "Create pull request"

Fork and committed branch

Step 16: Give your pull request a title and description
Pull request title and description 

Step 17: Click "Create Pull Request" button to initiate your pull request.
Create pull request button

Step 18: Once your pull request is complete copy the pull request ID from the title or the URL. 

Summary

Well done, you have sucessfully created your first pull request! You might be wondering what happens next? A common flow is for other developers to review your PR and then either directly approve it or provide some feedback for potential changes or queries they may have. Once you have approval it can then be merged into the main line. 
Tips

    Don't make your edits directly on the master branch, always create and checkout a fork before making changes

    Make sure you push your development branch to your fork

    You can select the current branch inside Github by clicking the branch dropdown

