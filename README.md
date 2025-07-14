* What is Vasion Control:
1. Version Control is a system that keep track and mange changes made to a file particularly source code over time.

* What is the use of Version Control:
* Version control systems allow multiple people to work on the same project simultaneously without overwriting each other's work. 
* They enable teams to merge changes from different developers, making it easier to combine individual contributions into a cohesive whole. 
* Tools like Git, GitHub, and GitLab provide features like branching, merging, and pull requests to streamline collaborative workflows. 

* What is GIT
* GIT is a distribution version control system that track version of system.

* What is GITHUB
* GITHUB is a webase plateform  that provid version control and collaboration tools for software developers.

* Different between GIT and  GITHUB
1. GIT:
* Git is managed by the Linux Foundation.
* Git is open source
* Git is installed locally
* Git is free;

2. GITHUB:
* GitHub is owned by Microsoft.
* GitHub is proprietary.
* GitHub is cloud-based.
* GitHub isn't.


* COMPREHENSIVE GIT AND GITHUB SETUP
* FOR GEGINNER:
* To get started with Git and GitHub as a beginner, you'll need to install Git, create a GitHub account, and then link the two. This involves initializing a local repository, adding files, stagingchanges, committing them, and then pushing to a remote repository on GitHub. 

1. Install GIT:
sudo apt install git 
Verify the installation by opening a terminal or Git Bash and typing git --version. 

2. Creat a GitHub Account:
Navigate to the GitHub website and create a new account.
Follow the prompts to set up your username, email, and password. 

3.  Configure Git:
* Open your terminal or Git Bash and Set your username and email. 
* git config --global user.name "Your Name"
* git config --global user.email "your.email@example.com"

* Start the ssh-agent in the background using.
* eval "$(ssh-agent -s)"
* > Agent pid 59566

* Add your SSH private key to the ssh-agent.
* ssh-add ~/.ssh/id-ed25519

* When you are prompted, touch the button on your hardware security key.
* When you are prompted to "Enter a file in which to save the key," press Enter to accept the default file location.
* When you are prompted to type a passphrase, press Enter.

* Add the SSH public key to your account on GitHub. 

* Before adding a new SSH key to your account on GitHub.com, complete the following steps.
1. Check for existing SSH keys.
2. Generate a new SSH key and add it to your machine's SSH agent.

Adding a new SSH key to your account:
1. Copy the SSH public key to your clipboard.
cat ~/.ssh/id-ed25519.pub
2. In the upper-right corner of any page on GitHub, click your profile picture, then click  Settings.
3. In the "Access" section of the sidebar, click  SSH and GPG keys.
4. Click New SSH key or Add SSH key.
5. In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal laptop, you might call this key "Personal laptop".
6. elect the type of key, either authentication or signing. 
7. In the "Key" field, paste your public key.
8. Click Add SSH key.
9. If prompted, confirm access to your account on GitHub.

* How to push:
1. Initialize Git (if not already done): Navigate to your project directory in the terminal and run:    git init
2. Add Files to Staging: Stage the changes you want to commit. To add all new or modified files:
    git add . 
3. To add specific files:
       git add <filename>
4. Commit Changes: Create a commit, which is a snapshot of your staged changes with a descriptive message:
          git commit -m "Your commit message"
5. Connect to Remote Repository (if not already done): If you are pushing to a new GitHub repository, you need to link your local repository to the remote one. Get the HTTPS or SSH URL from your GitHub repository and run:
             git remote add origin <remote_repository_url>
6. push Changes: Upload your committed changes from your local branch to the remote repository on GitHub:
           git push origin <your_branch_name>
* Git Pull: 
1. Fetch and Merge: To update your local repository with changes from the remote, including new commits and updates, run:
            git pull origin <your_branch_name>
