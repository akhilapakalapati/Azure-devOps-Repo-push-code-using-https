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


  # To push the updated code from the "tester" branch to Azure DevOps, you can follow these steps:

1. **Switch to the "tester" Branch**: First, ensure that you're on the "tester" branch by using the following command:

    ```bash
    git checkout tester
    ```

2. **Pull Changes from Remote (Optional)**: It's a good practice to pull any changes from the remote repository to ensure that your local branch is up to date before pushing your changes. You can use the following command:

    ```bash
    git pull azure tester
    ```

    This command fetches changes from the Azure DevOps repository and merges them into your local "tester" branch.

3. **Commit Your Changes**: Make any necessary changes to your code and then add and commit them as usual:

    ```bash
    git add .
    git commit -m "Your commit message"
    ```

4. **Push Changes to Azure DevOps**: Once your changes are committed, you can push the "tester" branch to Azure DevOps using the following command:

    ```bash
    git push -u azure tester
    ```

    This command will push your changes to the "tester" branch on the Azure DevOps repository.

By following these steps, you can successfully push the updated code from the "tester" branch to Azure DevOps. Let me know if you need further assistance!


