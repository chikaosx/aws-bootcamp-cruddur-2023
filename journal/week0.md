# Week 0 — Billing and Architecture

# AWS cridential
Here are the steps I have taken in creating an AWS root account, creating a user using IAM, activating change password on login, creating a group, giving the group administrator access, assigning a user to the group, and creating an Access key:

Create an AWS root account: I first created an AWS root account by signing up for an AWS account and providing the necessary information.

Create a user using IAM: After creating the root account, I created a user using IAM (Identity and Access Management) by navigating to the IAM console, selecting "Users," and clicking "Add user."

Activate change password on login: To ensure the security of the user's account, I activated the "Require user to change password on next login" option when creating the user. This will prompt the user to change their password the first time they log in.

Create a group: Next, I created a group by navigating to the IAM console, selecting "Groups," and clicking "Create New Group."

Give the group administrator access: To give the group administrator access, I selected the "AdministratorAccess" policy when creating the group.

Assign the user to the group: After creating the group, I assigned the user you created earlier to the group by navigating to the "Groups" section of the IAM console, selecting the group, and clicking "Add users to group."

Create an Access key: Finally, I created an Access key for the user by navigating to the "Security credentials" tab of the user's details page in the IAM console and clicking "Create access key." This Access key can be used to programmatically access AWS services and resources.

# AWS CLI
AWS cloudshell is a browser based shell that gives user command-line access to AWS resources
CLI is not available in every region, if it is not showing in top left corner of the dashboard change your region

I congfigured Auto Prompt using "aws --cli-auto-prompt"  command; Auto-prompt helps us to write CLI very quickly
i used "aws sts get-caller-identity" to check who I am and it prompted. this command is important to verify where you are deploying resources and you are not running on a wrong account when using multiple account. 

running this command "aws sts get-caller-identity" on my CLI will prompt this
{
    "UserId": "AIDA4FTW7USCUWGZPEBJ7",
    "Account": "836694418565",
    "Arn": "arn:aws:iam::836694418565:user/chika"
}

ARN is Amazon resource name

I used CLI command "aws account get-contact-information" to get my account information

# Installing AWS CLI on our repository
Go to github click on gitpod it will open shell then run CLI installation command
 curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
 run ls -la to view all the file downloaded
 
 i leant how to set enviroment variables using aws configure and how to use export
