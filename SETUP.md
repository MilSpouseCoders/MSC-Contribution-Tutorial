# Setup instructions

Here you will find instructions on what software and tools you will need to install on your personal machine in order to contribute to our repositories.

There are multiple ways to contribute to a repo and it's up to you to chose what you're most comfortable with. Don't let anyone tell you that your way is the wrong way, contributing and working together is the end goal, but for our projects here we are going to have a specific set of instructions for _beginners_ to follow. That way, if you have any questions about the process along the way, we can help you with that specific step more easily.

## Step 1: Create a GitHub account

<img alt="GitHub" src="https://desktop.github.com/images/desktop-icon.svg" width="100">

GitHub is an online service that stores code pushed to it from computers that have the Git installed. Git is a version-control system for tracking changes in source code. It shows what changed, what it was previously, who changed it, when it was changed, and why it was changed (because when we _commit_ (a fancy word for save) the changes, we write messages to explain the change). Git is a programmers best friend!

-   If you don't have one, go to [GitHub](https://github.com/) and create your free account.
-   There is a paid version, but if you're just starting out, free is all you need.

## Step 2: Download Visual Studio Code

<img style="left"  src="assets/visualstudiocodelogo.png" alt="clone this repository" width="200" />

**At this point if you have Git setup and you'd prefer to use a different editor (other than Visual Studio Code), you can use the either of the instructions below to contribute to our repository.**

-   For instructions on how to contribute via the **Command Line**, please go [here](command-line-tutorial.md).
-   For instructions on how to contribute via **GitHub Desktop**, please go [here](github-desktop-tutorial.md).

There are many code/text edititors and IDE's (integrated development environment) out there, but for this project and others we are recommending you download [Visual Studio Code](https://code.visualstudio.com/download).

-   Why are we asking you to do this? If you need help with something and you're using an editor we haven't used before, we're not going to be much help. That being said, if you're comfortable using another code editor, by all means, use it!

## Step 3: Set up Git

To install git, go to the official [Git website](https://git-scm.com/downloads) with instructions on how to get it on your machine. Installation is different for Mac and Windows, so you'll have to follow the instructions for your operating system.

CodeCademy has basic installation instructions on their website [here](https://www.codecademy.com/articles/git-setup). This article has instructions for both Windows and Mac.

If you aren't sure if you have Git, run the following command in the Terminal (Mac) or Command Prompt (Windows):

`git --version`

This command will check your machine to see if you have Git installed and if you do, what version you're running.

If you already have git, the command line will return the version number.

_For example:_

`git version 2.23.0`

## Step 4: VSC Integrated Terminal

Visual Studio Code has an integrated terminal (like most IDE's) and that's what we will be using when sending our code to GitHub.

### Here are 3 different ways to open the integrated terminal:

-   Click on the **_square button with the less than arrow inside_**.

    <img style="left"  src="assets/vsc_terminal1.png" alt="clone this repository" width="200" />

-   At the top of the IDE click **_Terminal -> New Terminal_**.

    <img style="left"  src="assets/vsc_terminal2.png" alt="clone this repository" width="200" />

-   Type **_ctrl \`_** (the back tick button, usually on the key with the ~ (tilde)).

Since you should now have Git installed on your machine, run the `git --version` command in your VSC terminal. It should return the version installed. If you get a version number returned, then good job!

## Step 4: Fork the Hackathon_2020 repository

Now that you have everything installed, head to your favorite web browser and fork a copy of this repository by clicking on the **fork** button on the top right of the main page of the repository [here](https://github.com/MilSpouseCoders/Hacktoberfest_2020). (You should be logged into your GitHub account.)

<img style="left" src="assets/step2_fork.png" alt="step 2" width="300">

This will create a copy of this repository in your personal GitHub account that you can now work with. There are open source repositories all over the place, this allows people to collaborate on programs and projects. So if you find other repositories you like, fork those and take a look at the code! The next step will tell you how to download that code onto your own machine so you can run the programs yourself.

## Step 5: Clone the Hackathon_2020 repository to your machine

Go to your _personal_ GitHub account and click on the forked copy of the repository that should now be listed. Click on the green **Code** button.

< src="assets/step3_code.png" alt="clone this repository" width="300" />

Click the _copy to clipboard_ icon or highlight and copy the listed url.

<img style="left" src="assets/step4_clone.png" alt="copy URL to clipboard" img width="300"  />

**In the Visual Studio Code integrated terminal run the following git command:**

```
git clone "url you just copied"
```

where "url you just copied" (without the quotation marks) is the url to your forked repository.

_For example:_

```
git clone https://github.com/this-is-you/hacktoberfest_2020.git
```

where `this-is-you` is your GitHub username. Here you're copying the contents of the hacktoberfest_2020 repository on GitHub to your computer.

As soon as the cloning process is finished, you the cloned files should be available to you in Visual Studio Code within the Explorer.

<img style="left" img width="300" src="assets/vsc_step5.png" alt="vsc file explorer" />

Click the arrow to the left of _Hacktoberfest_2020_ to look at the files. You have successfully cloned a repo to your machine!

**SET ORIGIN!**

## Step 6: Create a Branch

Before you do anything else, you're going to create a branch for you to work on. This way, you're not working on the master branch.

In the VSC integrated terminal, create a branch using the `git checkout` command:

```
git checkout -b <add-your-new-branch-name>
```

<img style="left" img width="600" src="assets/vsc_step6_1.png" alt="checkout branch" />

(The name of the branch does not need to have the word _add_ in it, but it's a reasonable thing to include because the purpose of this branch is to add your name to a list.)

This will automatically move you to your new branch. You're checking out the new branch you created!
You should now have 2 branches: a master branch and the branch you just created.

To check the branches type:

`git branch`

<img style="left" img width="300" src="assets/vsc_step6_2.png" alt="checkout branch" />

A list of the branches you currently have should appear. To exit out of the branch list, hit the **"q"** on your keyboard. That will "quit" you from the window and take you back to the terminal.

## Step 7: Make the necessary changes and Commit those changes

Now double click on the `first_duty_station.md` file to open it up in VSC. 

<img align="center" width="200" src="assets/vsc_step7_1.png" alt="git status" />

There are instructions at the top of the file on what you need to do. Make your addition to the file and **be sure to save it!** After you save the file you will see that the file itself in the file Explorer has changed colors.

<img align="center" width="600" src="assets/vsc_step7_2.png" alt="git status" />

In the integrated terminal, type the command `git status`, you'll see there are changes.

<img align="center" width="450" src="assets/step5_status.png" alt="git status" />

It says there are "changes not staged to commit" and to use "git add <file>" to update what will be committed. So lets do that!
To stage those changes to the branch you created, use the `git add` command:

```
git add first_duty_station.md
```

Now it's time to commit those changes using the `git commit` command:

```git commit -m "Add <your-name> to first_duty_station list"

```

replacing `<your-name>` with your name. The "-m" stands for message and the text in the quotes is the message. These messages are important, so always make sure you write thoughtful and consice messages about the changes you made to a file.

## Step 8: Push your changes to your GitHub

Now, you have to send the changes you made to your personal GitHub account.

Push your changes using the command `git push`:

```
git push origin <add-your-branch-name>
```

replacing `<add-your-branch-name>` with the name of the branch you created earlier.

## Step 9: Submit your changes for review

Now the goal is to get your changes added to the original repository that is maintained by someone else.

To do that go to your personal GitHub account, click _repositories_, and select the repository you're working with. You'll see a `Pull Request` tab at the top.

<img style="float: right;" src="assets/step7_pullrequest1.png" alt="create a pull request" width=600/>

Click on that tab and then click the green _Create Pull Request_ button.

<img style="float: right;" src="assets/step7_pullrequest.png" alt="create a pull request" width=600/>

Make sure it has a subject typed in and add any comments if necessary. Click _Create Pull Request_ one more time.

<img style="float: right;" src="assets/step7_pullrequest2.png" alt="submit pull request" width=600/>

That's it!
Soon we'll be merging all your changes into the master branch of this project. You will get a email notification once the changes have been merged.

## Where to go from here?

Congrats! You just completed the standard _fork -> clone -> edit -> PR_ workflow that you'll encounter often as a contributor!

## Additional info:

[More info on git installation and setup](https://docs.github.com/en/github/getting-started-with-github/set-up-git)
