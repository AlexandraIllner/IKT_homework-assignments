 You will demonstrate your understanding of GitHub remote workflows by forking a repository, making a meaningful change, and submitting a Pull Request (PR) to propose that change.

In the last lecture, you were introduced to:

• GitHub remotes and how they work
• Forking public repositories to your own GitHub account
• Cloning a remote repository locally
• Creating and switching branches
• Making commits and pushing changes
• Creating a Pull Request to propose your changes You also explored the prose-builder repository. This is the repo you'll be working with.

## Exercise 1

1. **Fork the Repository**

Go to the public prose-builder GitHub repository: https://github.com/bs-jokri/prose-builder

Click the Fork button to create your own copy under your GitHub account.

2. **Clone Your Fork**

Clone your forked repository to your local machine.
`git clone https://github.com/AlexandraIllner/prose-builder.git`

Set the upstream remote to the original prose-builder repository.
````
git remote add upstream https://github.com/bs-jokri/prose-builder.git
````

**Verify remotes with git remote -v**
`ala@ala-ThinkPad-P50:~/IdeaProjects/uni/IKT/prose-builder$ git remote -v`
`origin	https://github.com/AlexandraIllner/prose-builder.git (fetch)`
`origin	https://github.com/AlexandraIllner/prose-builder.git (push)`
`upstream	https://github.com/bs-jokri/prose-builder.git (fetch)`
`upstream	https://github.com/bs-jokri/prose-builder.git (push)`


3. **Create a Feature Branch**
Create a new branch named add-<your-name>-feature, e.g., add-readme-feature.
`git checkout -b add-AlexandraWeber-feature`

4. **Make a Contribution**

Choose one of the following:

• Add a new sample story or content file to the /samples/ directory.

• Fix a typo or improve formatting in the README.md file.

• Add a new utility function to an existing script (keep it simple).

• Add a new feature or improvement based on lecture discussion.

Commit your changes with a meaningful message.

5. **Push and Create Pull Request**
Push your feature branch to your GitHub fork.
`git push --set-upstream origin add-AlexandraWeber-feature`

Open a Pull Request (PR) to the original prose-builder repository’s main branch.

Include a short but clear description of your changes.
[pull request]:https://github.com/bs-jokri/prose-builder/pull/8

> ![[pullReq 2.png]]

## Exercise 2 
**Conceptual Questions**
1. Explain the difference between origin and upstream in a Git repository.
>*When forking a project and cloning the fork onto a local machine, one's own remote repository is set as* remote origin *(the local repo **originates from** there). The original project's repository (source of truth) to which we want to contribute can and should be set as* remote upstream*, so we can fetch/pull any changes to the original/source project while working on our contribution. When we create a pull request, we want to send our changes **"upstream to the source***


2. Why is it considered good practice to pull the latest changes from the upstream repository before creating a pull request?
>*1. Pulling the latest state of the upstream repo makes reviewing the pull request much easier. 2. In case upstream changes affect my work, I can handle it before creating the pull request.*

3. What are some advantages of using branches when collaborating on a project?
 >1. **The main branch is protected:** When features, bug fixes etc. are developed on branches, code on the main branch is not affected.
 >2. **Modules/features can be developed independently.** 
 >3. **Ideas can be tried out with no danger to the project.**
 

Submission Guidelines:

Please prepare one document as pdf, which contains the link to your Pull Request. Also add the answers to the questions in Exercise 2 to the document.

Tips:

You can always pull the latest changes from the original repository using: git pull upstream main



Keep your commits atomic and descriptive. e.g., fix: corrected typo in README




