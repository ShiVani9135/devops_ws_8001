# Git Hub Steps

1. First accept the invitation
2. Create a folder on your local system where you want to clone the repo
3. Do the cloning part
    `git clone `
4. After cloning is done that repo will be available in our local folder
5. Create a new branch in which we are going to push our files.
    `git checkout -b "feature-rosh12007" `
6. now add the files into that repo using git command 
  `git add .`
7. Check the status to see if git is tracking the changes or not 
    `git status`
8. Now commit all the changes with a proper message.
    `git commit -m "roshni.bcastudent23.12007@cimage.in (my first commit)" `
9. Now finally push it to github.
    `git push upstream ...`
(this i will get even when i do git push and the command will be vissible just copy and paste and finally enter to push it on the github.)

10. now finally our files are pushed on to github we can refresh and see this 


---
# EC2 Steps

1. first create your account on AWS website.
2. After creating the account search for EC2 in the search box there
3. Now a new page for EC2 will be available.
4. Click on the  **Launch instances** button and procede further.
5. after clicking the button a form will be appear to create a instance fill the form and finally click on **create instance** button.
    ```
    name: devops-3rd
    choose the os in my case *ubuntu*
    now choose the instance type (free one as we are not a paid user)
    key pair: devops-3rd (*if its already been create otherwise create one by clicking on the create a new key pair*)
     `in order to create a new keypair we need to provide a new name
     then don't do anything just left everything as it is by default and press **create new key** `

     after that click on the check box for http and ssh
     and finally 

     click on **create instance**

     ```

6. in our system a .pem file is created when we are creating the EC2

in cmd type `ssh -i filename.pem ubuntu@ipv4address

---
---

# Github action (CI/CD pipeline)

 ` code ---> build -->(secrets) github action
1. Make some changes in the code for example add comment and check for the status then commit with a message and finally push it.
2. make sure you create secrets on the github 
### to create this just goto settings select secrets from  the left hand side of the page and we will see a dropdown just click on action and create new secrets
    - EC2_HOST
        `ipv4 address`
    - EC2_USER
        `ubuntu`
    -EC2_SSH_KEY
        `paste all of the content we have downloaded using the EC2 launch in **.pem** file `

here we will connect from the AWS


                                   **Thankyou**

