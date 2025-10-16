# Shivam Singh BCA AKU B-1 310-22831 A-02 23-26

## All Git Steps:
1. Download [Git](https://git-scm.com/downloads) on your local machine.
1. Create a [GitHub](https://github.com/) account.
1. Config your git by using the following:
	1. ``git config --global user.name "Your Name"``
	1. ``git config --global user.email "your@mail.com"``
1. Create a new Repo on your GitHub.
1. Copy the ``https`` link of the Repo from GitHub.
1. Open git bash.
1. cd into your desire directory as ``cd <directory>``
1. Now git clone ``git clon <url that you just copied>``
1. Make changes to your codebase.
1. ``git status`` to check the status of your codebase.
1. ``git add <filename>`` to stage your changes for a file.
1. ``git add .`` to stage your all your changes.
1. ``git commit -m "<Your commit message>"`` to commit/save all the changes.
1. ``git push`` to sync all your changes to the GitHub.
## All EC2 steps
1. Create an AWS account.
1. Go to search bar.
1. Search for EC2 and select it.
1. Click on launch instance.
1. Create a name for your EC2 instance.
1. Select OS(Ubuntu is recommended).
1. Select AMI.
1. Select Instance type.
1. Key pair:-
	1. Select an existing one. OR
	1. Create a new one.
1. Select Network options
1. Select Storage Options.
1. Config your Domain setting.
1. Launch.
## GitHub Action
1. Go to your git repo ``cd <git/repo>``
1. Create a folder as: ``mkdir .github/workflows``
1. cd into the newly created directory ``cd .github/workflows``
1. Create a ``.yaml`` file
1. Write an action in your created ``.yaml`` file:-
1. A hello world example:
<pre>
name: main

on: push

jobs:
    say_hello:
        runs-on: ubuntu-latest
        steps:
            - name: Print a greeting
            run: echo "Hello World!"
</pre>
1. Commit the changes.
1. Push the changes.