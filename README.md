# Learn Git using Javascript30 Course
Practice Git using [wes bos JavaScript30 course](https://javascript30.com/)

## Step 1

In this step, we will fork this tutorial repository.

### Instructions

* On this current GitHub repository, scroll to the top and look for a button that says `fork`.
* Click the `fork` button.
  * <details>

    <summary> What does this do? </summary>
    <br />

    This will essentially copy all of the code from this repository, but make it as a new repository under your account. As you can imagine, you can't push directly to the DevMountain repo, because that would not be secure for DevMountain (anyone could make any changes they want). What you should do is create a fork of this repo, then push to your own fork because it's under your own account.

    </details>

## Step 2

In this step, we will take the forked repository and clone it down to our machine.

### Instructions

* Go to your forked repository on GitHub. It should appear under `Your repositories` which is next to the `New repository` button.
* Click on the green `clone or download` button and copy the URL.
* Open a terminal window and navigate to your Desktop.
* Run `git clone https://github.com/hafiziazmi/learn-github-js30.git`
  * <details>

    <summary> What does this do? </summary>

    <br />

    This takes what's on GitHub and essentially downloads it so you can now make changes to it on your local computer.

    </details>

## Step 3

In this step, we will make changes to our clone and push them to GitHub.

### Instructions

* Open the folder in your coding IDE.
* Make a change in a file.
* Open a terminal window and make sure it is in the directory of `learn-github-js30`.
* Run `git status`
  * <details>

    <summary> What does this do? </summary>

    <br />

    This will show what files have been changed. This also helps us determine what files we want to add to GitHub and what files we don't want to add to GitHub.

    </details>
* Run `git diff`
  * <details>

    <summary> What does this do? </summary>

    <br />

    This will show the actual code that has been changed. Again, we want to make sure we don't push anything to GitHub that shouldn't be there.

    </details>
* Run `git add .` OR `git add nameOfMyFile.fileExtension`
  * <details>

    <summary> What does this do? </summary>

    <br />

    This adds our file(s) to the 'staging area'. This is basically a fail safe if you accidentially add something you don't want. You can view items that our staged by running `git status`.

    </details>
* Run `git commit -m "The sentence I want associated with this commit message"`<br />
Adjust your message accordingly, eg:<br />
`git commit -m "Task for Day 02"`
  * <details>

    <summary> What does this do? </summary>

    <br />

    This tells your computer: 'Hey, the next time code is pushed to GitHub, take all of this code with it.' The message also specifies what GitHub will display in relation to this commit.

    </details>
* Run `git push origin main`
  * <details>

    <summary> What does this do? </summary>

    <br />

    Your code is now pushed to GitHub. Be sure to include `origin main`, as this tells GitHub which branch you want to push to, and creates the branch if it doesn't exist yet.

    </details>
* Go to your repository on GitHub and see your updates.

## Step 4

### Summary

Here is where things start to get different. Let's imagine we're working in groups. If we have everyone pushing to one repo without verifying the quality of the code, things can get messy pretty quick. GitHub fixed this solution with 'Pull Requests.' Basically, you fork a project, make changes to your fork, then you make a Pull Request (PR) back into the original project requesting that some piece of code be added to the original repo. This is how the vast majority of open source code projects work. In this step, we will make a pull-request.

### Instructions

* Go to your forked repo on GitHub.
* Locate the button that says `Pull Request` and click it.
* Locate the green button that says `New pull request` and click it.
  * You should now see the file changes you've made and how they differ from the original repo.
* Click on the `Create pull request` button to submit your PR.
* Now if you navigate to the <a href="https://github.com/hafiziazmi/learn-github-js30/pulls">original repository</a> and take a look at the `Pull Requests` yours should be there.