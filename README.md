# Software-Quality-Handbook

- **Iuliana**: Task estimation in Scrum _(3 resources)_ / Coding standards _(2 resources)_
- **Rosa**: Coding standards _(3 resources)_ / Code reviews _(2 resources)_
- **Jenkin**: Task estimation in Scrum _(2 resources)_ / Code reviews _(3 resources)_

500 - 1000 words per topic

## Guide to how we commit our work

### Main Branch

- This branch will be used to hold the final version of this project

### Develop Branch

- After we complete the work on a **feature branch** we merge it into the **develop branch**
- When merging **feature branches** into the **develop branch** we must:
  1. Make sure we are in the **develop** branch

        > git checkout develop

  2. Use **patching** to merge the folder from the **feature branch** with just one folder in the **develop branch**

        > git checkout --patch *feature-branch-you-want-to-merge* *folder-name-you-want-to-merge*

  3. At the question in command line choose **y** and press enter
  4. Stage these changes
        > git stage --all
  5. Commit a message with these changes
        > git commit -m "Merge message"
  6. Push these changes to the **develop branch**
        > git push origin develop
- Once all **feature branches** have been merged into the **develop branch** we merge it into the **main branch**

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
  - ***CodeReviews.md***
  - ***CodingStandards.md***
  - ***TaskEstimationInScrum.md***
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