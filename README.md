# Software-Quality-Handbook

- **Iuliana**: Task estimation in Scrum _(3 resources)_ / Coding standards _(2 resources)_
- **Rosa**: Coding standards _(3 resources)_ / Code reviews _(2 resources)_
- **Jenkin**: Task estimation in Scrum _(2 resources)_ / Code reviews _(3 resources)_

500 - 1000 words per topic

## Guide to how we commit our work

### Main Branch

The **main branch** will be used to hold the final version of this project.

### Develop Branch

- After we complete the work on a **feature branch** we merge it into the **develop branch**.
- When merging **feature branches** into the **develop branch** we must:
  1. Make sure we are in the **develop** branch

        > git checkout develop

  2. Use **patching** to merge the folder from the **feature branch** with just one folder in the **develop branch**

        > git checkout --patch *feature-branch-you-want-to-merge* *"folder-name-you-want-to-merge"*

  3. At the question in command line choose **y** and press enter
  4. Stage these changes

        > git stage --all

  5. Commit a message with these changes

        > git commit -m "Merge message"

  6. Push these changes to the **develop branch**

        > git push origin develop
        
- Once all **feature branches** have been merged into the **develop branch** we merge it into the **main branch** by doing a **pull request**.

### Feature Branches

- There are 3 different branches for each topic
  - ***code-reviews-feature***
  - ***coding-standards-feature***
  - ***task-estimation-feature***
- In each branch there is a folder for each topic
  - ***Code reviews***
  - ***Coding standards***
  - ***Task estimation in Scrum***
- In each folder there is a file for each topic
  - [***CodeReviews.md***](/Code%20reviews/CodeReviews.md)
  - [***CodingStandards.md***](/Coding%20standards/CodingStandards.md)
  - [***TaskEstimationInScrum.md***](/Task%20estimation%20in%20Scrum/TaskEstimationInScrum.md)
- When editing a file we must:
  1. Make sure we are in the correct **feature branch**

        > git checkout *feature-branch-name*

  2. Then we can make changes to the file in Visual Studio Code - to open:

        > code .

  3. Once completed, stage all changes 

        > git stage --all

  4. Commit a message with these changes

        > git commit -m "File updated"

  5. Push these changes to the specific **feature branch**

        > git push origin *feature-branch-name*


## If we were to do this project again, what would we do different?

### Create our own branches
- From the feature branches we would each create our own branch
- That way we wouldn't have to worry about conflicts when editing or pushing changes to the same file
- When merging we would first merge the files from our own branch to the feature branch and then merge the feature branches as mentioned above

### Create just the files
- Instead of having folders and inside those folders have the files, we would create just the files for each topic
- That way the structure of the project would be more simple

### When creating feature branches, keep them the same as the develop branch
- When we created our feature branches we kept just the relevant folder in each branch
- This resulted in us having to use patching when merging the feature branches into the develop branch to avoid folder deletion
- If we were to keep the feature branches the same as the develop branch we would have been able to do normal pull requests from the feature branches
