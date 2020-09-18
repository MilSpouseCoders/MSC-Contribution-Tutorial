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
- For instructions on how to contribute via the **Command Line**, please go [here](command-line-tutorial.md). 
- For instructions on how to contribute via **GitHub Desktop**, please go [here](github-desktop-tutorial.md).

There are many code/text edititors and IDE's (integrated development environment) out there, but for this project and others we are recommending you download [Visual Studio Code](https://code.visualstudio.com/download).
-   Why are we asking you to do this? If you need help with something and you're using an editor we haven't used before, we're not going to be much help. That being said, if you're comfortable using another code editor, by all means, use it!


## Step 3: Set up Git

To install git, go to the official [Git website](https://git-scm.com/downloads) with instructions on how to get it on your machine. Installation is different for Mac and Windows, so you'll have to follow the instructions for your operating system.

CodeCademy has basic installation instructions on their website [here](https://www.codecademy.com/articles/git-setup). This article has instructions for both Windows and Mac.

If you aren't sure if you have Git, run the following command in the Terminal (Mac) or Command Prompt (Windows):

```git --version```

This command will check your machine to see if you have Git installed and if you do, what version you're running. 

If you already have git, the command line will return the version number.

_For example:_

```git version 2.23.0```

## Step 4: VSC Integrated Terminal

Visual Studio Code has an integrated terminal (like most IDE's) and that's what we will be using when sending our code to GitHub.

### Here are 3 different ways to open the integrated terminal:

- Click on the **_square button with the less than arrow inside_**. 
<img style="right"  src="assets/vsc_terminal1.png" alt="clone this repository" width="200" />

- At the top of the IDE click **_Terminal -> New Terminal_**.
<img style="right"  src="assets/vsc_terminal2.png" alt="clone this repository" width="200" />

- Type **_ctrl \`_** (the back tick button, usually on the key with the ~ (tilde)).

Since you should now have Git installed on your machine, run the ```git --version``` command in your VSC terminal. It should return the version installed. If you get a version number returned, then good job!

## Step 4: Fork the Hackathon_2020 repository

Now that you have everything installed, head to your favorite web browser and fork a copy of this repository by clicking on the **fork** button on the top right of the main page of the repository [here](https://github.com/MilSpouseCoders/Hacktoberfest_2020). (You should be logged into your GitHub account.)

<img style="left" src="assets/step2_fork.png" alt="step 2" width="300">

This will create a copy of this repository in your personal GitHub account that you can now work with. There are open source repositories all over the place, this allows people to collaborate on programs and projects. So if you find other repositories you like, fork those and take a look at the code! The next step will tell you how to download that code onto your own machine so you can run the programs yourself.

## Step 5: Clone the Hackathon_2020 repository to your machine

Go to your *personal* GitHub account and click on the forked copy of the repository that should now be listed. Click on the green **Code** button.

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

## Step 6:
