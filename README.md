# Reflection on Branch Management and Collaboration Using Git

During this exercise, I followed a structured workflow to create and manage branches, simulate a merge conflict, and resolve it through Git’s pull request process.

## Creating and Managing Branches

I began by creating a feature branch named `feature/header` using:<br>
git checkout -b feature/header.

Within this branch, I created an index.html file and added a basic header section. I staged and committed the changes with:<br> 
git add index.html<br>
git commit -m "Added header section to index.html"<br>

After that, I switched back to the main branch and created a second branch called feature/footer to work on the footer section. I edited the same index.html file to add a footer element, then staged and committed the changes.

## Handling Merge Conflict
To simulate a merge conflict, I switched back to the feature/header branch and I didn't have the footer html in this file. This caused an intentional conflict when merging both feature branches back into main.

After merging feature/footer into main:<br>
git checkout main<br>
git merge feature/footer

I attempted to merge feature/header: <br>
git merge feature/header

This resulted in a conflict. I opened index.html, resolved the conflict manually, then used the following commands to complete the process:<br>
git add index.html<br>
git commit<br>

## Using Pull Requests for Code Quality and Collaboration

After resolving the conflict, I pushed my changes to GitHub using:<br>
git push origin main

I then opened a pull request. This allowed for a code review process that helps ensure code quality and promotes collaboration. It provided a chance to verify that all changes were correct and aligned with project goals.

<b>This exercise helped me understand the importance of structured branch management, conflict resolution, and using pull requests to maintain clean and collaborative code in a shared repository environment.<b>


