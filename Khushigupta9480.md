# DevOps Workshop 

## 1. Git Steps

-Install Github and create an account. 
-Install Gitbash on local if not installed and configure Git:
    git config --global user.name "Your user name"
    git config --global user.email "your_email@example.com"
-Create a New Repository on Github:
    Repo Name,
    public or private Repo,
    Add a Readme or not,
    .gitignore file,
    And finally create the Repository
-Create a new folder on your local 
-Inside the folder, Open GitBash Terminal
-Copy the HTTPS URL of your created repo and Clone the repo through GitBash:
    git clone <repo-url>
-Change Directory
    cd <repo_name>
-Make changes to existing code, you can add new files or edit existing files.
-Check Status for untracked files
    git status
-Add, Commit and Push Changes
    git add .
    git commit -m "Message"
    git push

## 2. AWS Instance Creation

-Create an AWS Account
-Login to AWS Console
-Navigate to EC2 Service
-Click Launch Instance
-Choose:
    -Name of instance
    -Operating System ( we chose ubuntu )
    -Amazon Machine Image( AMI ): ubuntu server
    -Instance Type: micro, nano, etc ( Free Tier by default )
    -Key Pair: Create key pair of RSA type and .pem file & Download .pem file
    -Security Group: Allow SSH, HTTP, HTTPS
-Launch Instance

## 3. GITHUB Actions

-Created a YAML File and push along with code on Github Repo.
-Within Github: Settings -> secrets -> Create Secret Keys
    -EC2_HOST: Public IPv4 Address of created instance
    -EC2_USER: ubuntu
    -EC2_SSH_KEY: Copy and Paste .pem file

## Finally, Check the running of CI/CD Pipeline

-Changes in the existing code
-git add .
-git commit -m "Changes"
-git push
-Go to Github Actions and see the running.