# GitHub Tutorial

_by Denia Casimiro_

---
## Git vs. GitHub

*Git:* Is a version control system that runs in the command line that a system that lets you manage and keep track of your source code history. Such as editing, removing, renaming and etc. One of the biggest different is that Git can be used _without_ having Github.

*GitHub:* Is a cloud-based hosting service that lets you manage Git repositories. Saving all your code in the Cloud. This tool is very useful during collaborate with other coders, this tool also let you be able to interact with other Repositories and be able to see the changes of their project. If you have open-source projects that use Git, then GitHub is designed to help you better manage them. Plus Github _does_ require GIt.


---
## Initial Setup

Ready to start coding! But don't know how to make an account! Don't worry I got you! To be able to use https://ide.cs50.io/, you will have to create an account in https://github.com/.
1. Go to https://github.com/
2. Click on "**Sign up**" on the top right corner of the Main Page
3. **Create an account** There you will bring to a page that will let you enter your username, passwords and email. (_You can use your school email or your own personal email_)
4. After you **confirmed** everything with your account, go to https://github.com/hstatsep/ide50 and follow the steps stated there.

*What is SSH key? & Why do we need to set up an SSH key between cs50 and GitHub?*

SSH key is a way for your local and remote to be able to connect. Also the SSH key is a shortcut that generated an alternate route to identify yourself without having you type in your username and password every single time.


---
## Repository Setup
Wanna create a repo? but dont know how? Don't worry I'll help you!

1. Now let get started,  **create a directory**. You can name it whatever you like, but I’d recommend calling it “first-repo”. Do this by typing in `mkdir "first-repo"` You can practice your code on your very first repo.
2. Make a `mkdir "first-repo"` into a repository, firstly, you need to **go into the directory** by doing `cd first-repo` and then secondly do `git init` to **initialize git**. Thirdly, after typing in `mkdir "first-repo"` you need to type in `cd "first-repo"` and then finally type in  `git init`. It should look like

         * `mkdir first-repo`
         * `cd first-repo`
         * `git init`

1. In the upper-right corner of any page, use the  drop-down menu, and select New repository.
2. Type a short, memorable name for your repository. For example, "first-repo".
3. Optionally, add a description of your repository. For example, "My first repository on GitHub." or "First Repo Code"
4. Choose to make the repository either public or private.
5. Select Initialize this repository with a README.
6. Click Create repository.

Congratulations! You've successfully created your first repository, and initialized it with a README file.

---
## Workflow & Commands
There are many Git workflows out there. A Git Workflow is a recipe or recommendation for how to use Git to accomplish work in a consistent and productive manner. Git offers a lot of flexibility in how users manage changes. Given Git's focus on flexibility, there is no standardized process on how to interact with Git.



---
## Rolling Back Changes
Even the fastest coders do make some mistakes, and that's okay! But if you made a mistake and don't know how to fix it? Don't worry!
1. ALWAYS READ YOUR CODE BEFORE CONFIRMING ANYTHING!
2. Even when you add an extra/miss a letter, you can retype the code again
3. But if you want to rename a file, you can used mv ,but you need to be outside of your file in order to do any renaming

If there's anything you want to remove the file and everything in the file itself, you can used ( rm -rf )