[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.png?v=103)](https://github.com/ellerbrock/open-source-badges/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

# Making your first contribution using the command line

## 1. Complete steps 1-3 in README.MD

Be sure you have completed steps 1 - 3 in the [README.MD](README.md) file.

## 2. Fork this repository

Fork this repository by clicking on the **fork** button on the top right of the main page of the repository [here](https://github.com/MilSpouseCoders/Hacktoberfest_2020).
This will create a copy of this repository in your personal GitHub account.

<img style="left" src="assets/step2_fork.png" alt="step 2" width="300">

## 3. Clone the repository

Go to your personal GitHub account and click on the forked copy of the repository that should now be listed. Click on the green **Code** button.

<img style="left"  src="assets/step3_code.png" alt="clone this repository" width="300" />

Click the _copy to clipboard_ icon or highlight and copy the listed url.

<img width="300" src="assets/step4_clone.png" alt="copy URL to clipboard" />

Open a Command Prompt (Windows) or Terminal (Mac )and run the following git command:

```
git clone "url you just copied"
```

where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

For example:

```
git clone https://github.com/this-is-you/hacktoberfest_2020.git
```

where `this-is-you` is your GitHub username. Here you're copying the contents of the hacktoberfest_2020 repository on GitHub to your computer.

## 4. Create a branch

Change to the repository directory on your computer (if you are not already there):

```
cd hacktoberfest_2020
```

Now create a branch using the `git checkout` command:

```
git checkout -b <add-your-new-branch-name>
```

For example:

```
git checkout -b add-jane-smith
```

(The name of the branch does not need to have the word _add_ in it, but it's a reasonable thing to include because the purpose of this branch is to add your name to a list.)

## 5. Make necessary changes and commit those changes

Now open `first_duty_station.md` file in a text editor, and follow the instructions on what to do. 

*Be sure to save the file.*

If you go to the project directory and execute the command `git status`, you'll see there are changes.

<img align="center" width="450" src="assets/step5_status.png" alt="git status" />

Add those changes to the branch you just created using the `git add` command:

```
git add first_duty_station.md
```

Now commit those changes using the `git commit` command:

```
git commit -m "Add <your-name> to first_duty_station list"
```

replacing `<your-name>` with your name.

## 6. Push changes to GitHub

Push your changes using the command `git push`:

```
git push origin <add-your-branch-name>
```

replacing `<add-your-branch-name>` with the name of the branch you created earlier.

## 7. Submit your changes for review

Now go to your personal GitHub account, click *repositories*, and select the repository you're working with. You'll see a `Pull Request` tab at the top.

<img style="float: right;" src="assets/step7_pullrequest1.png" alt="create a pull request" width=600/>

Click on that tab and then click the green *Create Pull Request* button.

<img style="float: right;" src="assets/step7_pullrequest.png" alt="create a pull request" width=600/>

Make sure it has a subject typed in and add any comments if necessary. Click *Create Pull Request* one more time.

<img style="float: right;" src="assets/step7_pullrequest2.png" alt="submit pull request" width=600/>

That's it! 
Soon we'll be merging all your changes into the master branch of this project. You will get a email notification once the changes have been merged.

## Where to go from here?

Congrats! You just completed the standard _fork -> clone -> edit -> PR_ workflow that you'll encounter often as a contributor!

## Additional info:

[More info on git installation and setup](https://docs.github.com/en/github/getting-started-with-github/set-up-git)
