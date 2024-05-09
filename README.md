# Azure-devOps-Repo-push-code-using-https
Creating new branch like tester/stage

To push your code to an Azure DevOps Git repository, you'll need to set up a remote for your Azure repository and then push your code to it. Here's a step-by-step guide:

1. **Get Azure DevOps Repository URL**: First, you need to obtain the URL of your Azure DevOps Git repository. You can find this URL by navigating to your repository in Azure DevOps.

2. **Add Azure DevOps Repository as Remote**: In your local Git repository directory, use the following command to add the Azure DevOps repository as a remote. Replace `<Azure_Repo_URL>` with the URL you obtained in step 1.

    ```bash
    git remote add azure <Azure_Repo_URL>
    ```

Azure_Repo_URL get Url from clone

------------------------------------------------------------------------------------------------------------------------------
To push to main 

3. **Push Your Code**: Once you've added the Azure repository as a remote, you can push your code to it using the following command:

    ```bash
    git push -u azure main
    ```


----------------------------------------------------------------------------------------------------------------------------------------

To push th code to other branches (create and push code):

1. **Create a New Branch**: Use the following command to create a new branch named "tester" in your local repository:

    ```bash
    git checkout -b tester
    ```

2. **Commit Your Changes**: Make your changes and commit them to the "tester" branch using `git add` and `git commit` commands.

3. **Push the New Branch**: Once your changes are committed, you can push the "tester" branch to Azure DevOps using:

    ```bash
    git push -u azure tester
    ```

    -----------------------------------------------------------------


