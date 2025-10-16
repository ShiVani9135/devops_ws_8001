
# NAME-AKHIL ,ROLL-a16,BCA3RD YEAR


# 🧠 Git, AWS EC2 & GitHub Actions — Step-by-Step Guide

---

## 🧩 1. GIT — Upload Local Code to GitHub

### Steps
1. Create a new repository on GitHub and copy the repository URL.  
2. Create a folder on your system and open **Git Bash** inside it.  
3. Clone the repository:  
   ```bash
   git clone <repository-url>
Go inside the cloned folder and paste your development code.

Check repository status:

bash
Copy code
git status
Stage all files:

bash
Copy code
git add .
Commit changes:

bash
Copy code
git commit -m "Initial project upload"
Push code to GitHub:

bash
Copy code
git push origin main
Note:
If you’re using Git for the first time, configure your username and email:

bash
Copy code
git config --global user.name "YourUsername"
git config --global user.email "youremail@example.com"


☁️ 2. AWS — Launch and Access an EC2 Instance
Steps
Log in to AWS Console.

Search for EC2 and click Launch Instance.

Give your instance a name.

Select an Amazon Machine Image (AMI) — e.g., Ubuntu 22.04 LTS.

Choose instance type: t2.micro (Free Tier).

Create or use an existing key pair (.pem or .ppk).

Launch the instance and wait until it’s running.

Access the EC2 instance using SSH:

bash
Copy code
ssh -i "keypair.pem" ubuntu@<your-ec2-public-ip>


⚙️ 3. GitHub Actions — Automate Deployment to EC2
Steps
Go to your GitHub repository → Settings → Security → Secrets and Variables → Actions.

Add the following repository secrets:

Secret Name	Secret Value	Description
EC2_HOST	Public IP of EC2	Example: 13.233.145.23
EC2_USER	ubuntu	Default EC2 username
EC2_SSH_KEY	Paste your full PEM key content	SSH private key for EC2 access

Check the Actions tab to ensure the workflow runs when you push code.

🧾 Summary

Tool	Purpose	Example Command

Git	Version control	git add ., git commit, git push
AWS EC2	Host apps in the cloud	ssh -i key.pem ubuntu@ip
GitHub Actions	CI/CD automation	Secrets + Workflow YAML