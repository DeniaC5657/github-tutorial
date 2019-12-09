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
Now that we have a README.md file, we can start typing in this file!
1. Now, make sure that we are inside the blank README.md file.
2. Secondly type in "My first repository."
3. Thirdly, that we have some text in the README.md file, let's click on the first-repo tab.
4. Fourthly, you should be in the terminal, type in `git add .`
(This command adds the file README.md  and its edits to the stage, also recored everything you edit or change. )
5. Now that we have added everything to the stage, let's commit it. Type in `git commit -m "add text to first-repo"`
( This command does is it "captures a photo of the stage" or records the change you have done before by naming it "add text to first-repo". Basically, in the future, you want to get something back that you may be deleted in the past, you can type in `git log` to get to see all the commits you've done and get the one you'd like back)
6. Now, in order to a command known as `git push`, we'll have to create our remote repo in order to push the text we have in our file somewhere and we need to go through some other steps first.

## _Git Push_

  * Now, open up a new tab and go to http://github.com/
  * Go to the top left corner and locate the green button that has a little book and reads "New", then click on it.
  * Type in the repository name. Such as type in _first-repo_ *_exactly_* the _same_ as you have it named.
  * When you're done, you can include a description if you would like to, but you don't have to. It not required.
  * Skip the _last step_, because we already have a README file in our first-repo that we made in our ide.cs50.
  * Click on the green button _Create Repository_

What does the command`git add remote origin (URL)` do?

        This command sets up a connection between our repository in our CS50 IDE and the new repository that lives on GitHub, saving every code that we put inside. The URL should be github.com:_yourusername_/first-repo.git

What does the command `git push -u origin master` mean?

        This command is done in order to send any changes or edits we've made from our local CS50 IDE to our remote repo which is on GitHub. The -u means upstream means that it will remember to push our changes to our remote repo whenever we type in `git push` in the future. Pushing everything we did and saving it so we use it in the future.

 * Make sure you are in your _first-repo_. Copy those 2 lines of code and then paste them into your command line in the CS50 IDE.
   * Now go back to github and refresh the page. You should see "My first repository."
   * Keep adding any text you'd like and repeat using git add, git commit, and git push.

There you go! You learn three new commands!


---
## Rolling Back Changes

Even the fastest coders do make some mistakes, and that's okay! But if you made a mistake and don't know how to fix it? Don't worry!
In order to get rid of any changes we would have to do the command `git checkout --<file>...`
## _How do you undo an edit?_
* To undo an edit you’ll have to type in the command `git checkout --filename`.

## _How do you undo a commit?_
* To  undo a commit you would need to type, `git reset --soft HEAD~1`. This command will delete the last commit you've made and reset to a past commit you would like back. This is a very useful tool to see what you did during your code.

## _How do you undo something you have added to the stage?_
* To undo something you have added on the stage you’ll have to type in `git reset HEAD filename`.

## _How do you undo something that you have pushed already?_
*  To undo a push commit you can do `git revert`. You could also do `git reset --hard HEAD~1` to remove 1 or multiple commits you have made in the past. But do check you’re undoing a correct push.

## _How do you undo a commit, something you've added to the stage, and an edit?_
* By doing `git reset --hard HEAD~1` you will be deleting the things you've just added to the stage and any uncommitted changes.


And that's it! You got the basics down! This is only the beginning! Start coding and having fun!