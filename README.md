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

* It should say `~/first repo/ (master)`
Now let's create a README.md file inside so that you're able to type any code you'll like in README.md file.

1. Firstly, type in `touch README.md` to create a new blank file inside our directory named README.md
          It should look like `~/first repo/ (master) $ touch README.md`
  2. Secondly, type in `c9 README.md` to go open this file in a new tab in your ide.cs50
          It should look like  `~/first repo/ (master) $ c9 README.md`
  3. Thirdly, it should now see 2 tabs next to each other and you should be in the blank README.md file.

To save this file, (On MAC) You can either click on File > Save or command + S or (On a PC) Ctrl + S
(Both way should change the red dot to the color green_)


Congratulations! You've successfully created your first repository, and initialized it with a README file.

---
## Workflow & Commands
There are many Git workflows out there. A Git Workflow is a recipe or recommendation for how to use Git to accomplish work in a consistent and productive manner. Git offers a lot of flexibility in how users manage changes. Given Git's focus on flexibility, there is no standardized process on how to interact with Git.



---
## Rolling Back Changes

Even the fastest coders do make some mistakes, and that's okay! But if you made a mistake and don't know how to fix it? Don't worry!
In order to get rid of any changes we would have to do the command `git checkout --<file>...`
##### How do you undo an edit?
* To undo an edit you’ll have to type in the command `git checkout --filename`.

##### How do you undo a commit?
* To  undo a commit you would need to type, `git reset --soft HEAD~1`. This command will delete the last commit you've made and reset to a past commit you would like back. This is a very useful tool to see what you did during your code.

##### How do you undo something you have added to the stage?
* To undo something you have added on the stage you’ll have to type in `git reset HEAD filename`.

#####  How do you undo something that you have pushed already?
*  To undo a push commit you can do `git revert`. You could also do `git reset --hard HEAD~1` to remove 1 or multiple commits you have made in the past. But do check you’re undoing a correct push.

##### How do you undo a commit, something you've added to the stage, and an edit?
* By doing `git reset --hard HEAD~1` you will be deleting the things you've just added to the stage and any uncommitted changes.


And that's it! You got the basics down and it's up to you! This is only the beginning!