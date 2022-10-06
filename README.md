# Using git and GitHub for Class Assignments

A video demonstration of the steps in this assignment is available at: https://youtu.be/4WVnIdRdWFw

Git is a version control system which runs on your computer. GitHub is an online location for creating and hosting remote repositories. ( https://github.com/ ) Version control systems and remote repositories were created for software development. However remote repositories like GitHub have become an easy way for programmers and other knowledge workers to share information. A great deal of teaching and learning materials are made widely available through GitHub repositories. This includes a lot of resources for statistics and data science. Since so much material you encounter online may be available through GitHub repositories and because online repositories make collaborating on work with other people so easy I have incorporated GitHub into the workflow for this course. We will be using GitHub in this course as a place where you can store your own copy of the assignments we will be completing. Rather than turn files in directly to our course software, you will upload your completed assignments to your GitHub repository for that assignment and turn in the link to your repository so I can go look at it there. I think this arrangement offers some benefits for everyone.

* You get an instaneous copy of the assignment in your own GitHub account.
* You will have access to your work from this class after this semester is over without a lot of work to archive it and put it online. It will be handy should you ever want to review it in the future.
* You will become familiar and more comfortable with how GitHub repositories work. Should you run across learning materials on GitHub in the future you will know how to access them and create your own copies.
* I can access your work quickly and easily using this method.

Since this is a statistics course and not a computer science course, I don't care if you have a deep knowledge of git. All you really need to know for this course is that it allows you to create copies of your GitHub repositories on your own computer. And when you make changes to files in your repositories which are linked to the remote version online, it can help you push those changes to your online version. If you want to learn more about the foundations and inner workings of git you can look through the Optional Material section at https://github.com/cmcntsh/compSci2021_Setup . (You don't need to do that for this class. I just provide the link in case you have interest.) Git started out as a command line program. We won't be using it that way in this course. But if you want to get a taste of how git works from the command line you can complete the exercises at https://github.com/cmcntsh/exerGitPractice . (You don't need to do that for this class. I just provide the link in case you have interest.)

## Fork this Repository

When you fork a GitHub repository, you create an exact copy of that repository on your own GitHub account. There are a couple things you should remember about forking repositories.

* You can only fork a repository (create a copy of the original repository in your own GitHub account) once. If you try to fork a repository again, you will get a message telling you that you already forked the repository. 
* You can't fork a repository which is already on your own account. (Other people can fork your repositories, but you can't fork your own repository to the same account.) If you try to fork a repository on your own account, you will get a message telling you that you can't fork your own repository.

Try it out by forking this repository to your own account.

* On this current GitHub repository, scroll to the top and look for a button that says `fork`. As of the time I wrote this, that button was at the top right corner of the page. It looks like the screenshot below. Click the button.

![Fork Screenshot](https://github.com/cmcntsh/gitHubForClassAssignments/blob/main/images/forkImage.png?raw=true)

That's about it. You should now have a copy of the repository with the same name in your own GitHub account. You should be able to tell the difference between the original and your copy by looking at the url address. The original will have my GitHub account name in the path. (Look for `cmcntsh`.) `https://github.com/cmcntsh/gitHubForClassAssignments` Your copy should have your username somewhere in the url instead of mine. (If you need help with this, post a question on the discussion board or come to office hours.)

## You can download and upload files directly from your repository on GitHub

Technically, you don't even have to clone the repository to your computer to complete and turn in your assignments. (I'll talk about what cloning the repository is a little further below.)

### Download files without cloning

You can download the files from your repository to your computer without cloning.

* On your own GitHub repository for this assignment, scroll up on the page and click on the green `Code` button. Then click on the `Download ZIP` button at the bottom of the dropdown menu. See screenshot below.

![Download Screenshot](https://github.com/cmcntsh/gitHubForClassAssignments/blob/main/images/downloadZip.png?raw=true)

* You should see the zip file download to your computer.
* Extract the zip folder and you should find all the files from the repository on your computer.

### Upload files directly to GitHub

You can manually upload files to GitHub. (If you didn't clone the repository, you will need to do this to put your completed assignment files into your online repository.)

* On your own GitHub repository, scroll up on the page and click on the `Add file` button next to the `Code` button. Then click on the `Upload files` button at the bottom of the dropdown menu. See screenshot below.

![Upload Screenshot](https://github.com/cmcntsh/gitHubForClassAssignments/blob/main/images/GitHubUpload.png?raw=true)

* After you drag your files or select them using the file chooser, click the green `Commit changes` button at the bottom of the screen.

After you load your completed assignment files to your online repository, you can turn in the link to your assignment repository in our course software.

## Clone your repository using RStudio

Cloning your repository means creating a copy of your GitHub repository on your own computer which is linked to your GitHub repository (aka the remote repository). You can do this using git commands in the command line (see https://github.com/cmcntsh/exerGitPractice), but it's a lot simpler using RStudio. To use the instructions below you need to have git and RStudio already installed on your computer.

* On your own GitHub repository for this assignment, scroll up on the page and click on the green `Code` button. Then click on the copy button at the top of the dropdown menu. It's right next to the little window that has the path. See screenshot below.

![Download Screenshot](https://github.com/cmcntsh/gitHubForClassAssignments/blob/main/images/downloadZip.png?raw=true)

* Create a new folder on your machine where you want to put this repository if you don't already have one you want to use.
* In RStudio go to File - New Project... - Version Control - Git 
  * Paste the repostory URL you just copied into the Repository URL: window.
  * You can use the name suggested in the Project directory name: window or enter a new one (no spaces in the name).
  * Click the Browse... button next to the Create project as subdirectory of: window and navigate to the folder where you want to keep your repository and click Open.
  * Check the Open in new session checkbox. (Bottom left corner of New Project Wizard popup.)
  * Click Create Project
* A new folder for your repsitory will be created inside the folder you selected.
* A new RStudio window should open showing the files in the repository folder in the Files tab of the bottom left pane in RStudio.

## Push changes to your GitHub repository using RStudio

Once you have the repository on your computer, you can complete your assignment using RStudio and Jamovi. Make sure you save your completed assignment files in your assignment repository folder on your computer. You can use RStudio to push changes in your repository to your remote repository in GitHub.

* (Instructions from: https://resources.github.com/github-and-rstudio/)
* In RStudio click the Git tab in the upper right pane.
* Click Commit.
* In the Review changes view, check the staged box for all files.
* Add a commit message, for example "Upload completed assignment".
* Click Commit.
* Click the Pull button to fetch any remote changes.
* Click the Push button to push your changes to the remote repository.
* On GitHub, navigate to the Code tab of the repository to see the changes.

## Turn in the Assignment Link

* Once you have forked this assignment to your own GitHub account and read through these instructions, create a new text file on your computer called `GitHubForAssignments.txt`.
* Write a short description of which method you think you will use to put your completed assignments on GitHub in the text file and save it to your computer.
* Use your preferred method to load the text file to your GitHub repository for this assignment.
* Turn the link to your assignment repository in.
* If you have question or run into problems, post a question on the discussion board for this week, or come to office hours. Remember screenshots of where you're having difficulty are helpful for everyone so they can provide good feedback.
