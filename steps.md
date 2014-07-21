##Updating Github Steps

This guide assumes that you have installed and set-up git already.

1) Set-up new repository on github.com (for this example I called it repoexample) and initialize it with a readme file (there's a checkbox).

2) Create a new folder on computer where you want to store the file (I recommend calling it the same as your remote, but it could be called something different). To do so using the terminal type:
	mkdir ~/repoexample

3) Go to the new directory: *NOTE:* All subsequent steps need to be executed while in this directory
	cd ~/repoexample

4) Initialize an empty local git reporsitory in this directory:
	git init

5) Link git repository to remote repository
	git remote add origin https://github.com/schweitzerb/repoexample.git

6) Get all the stuff from the remote. *NOTE:* This step is not mentioned ANYWHERE in the course documents, but it is necessary. If you don't do this, you'll get error messages at step 10 later because the local and remote repositories were not in sync. If you've had trouble getting this the HelloWorld.md file uploaded on github, this is most likely why.
	git pull origin master

7) Create and save the "HelloWorld.md" textfile in your repository. You can do this using the "TextEdit", just make sure the format is plain text "Format -> Make Plain Text" before you save.

8) Add the new file to be tracked to git
	git add .

9) Commit the change to your repository
	git commit -m "Adding helloworld.md"

10) Push the changes to the github remote repository


