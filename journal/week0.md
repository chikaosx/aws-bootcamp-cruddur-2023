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
Here are the steps you have taken in using AWS CloudShell, configuring auto-prompt, checking your identity, and installing AWS CLI into Gitpod:

Use AWS CloudShell: You started by using AWS CloudShell, which is a browser-based shell that gives you command-line access to AWS resources.

Check CLI availability: You noted that the CLI may not be available in every region, so you checked to see if it was available in your current region.

Configure Auto Prompt: You configured Auto Prompt using the "aws --cli-auto-prompt" command. This will help you write CLI commands more quickly by automatically prompting you for the required input.

Check your identity: You used the "aws sts get-caller-identity" command to check who you are and ensure that you are not running on the wrong account when using multiple accounts. This command returned your user ID, account number, and ARN.

Get account information: You used the "aws account get-contact-information" command to get your account information, which could include your account name, address, and contact information.

Install AWS CLI into Gitpod: Finally, you installed AWS CLI into Gitpod, which is a cloud-based development environment. This will allow you to use AWS CLI commands directly from Gitpod, without having to use CloudShell or any other command-line interface.

running this command "aws sts get-caller-identity" on my CLI will prompt this
{
    "UserId": "AIDA4FTW7USCUWGZPEBJ7",
    "Account": "836694418565",
    "Arn": "arn:aws:iam::836694418565:user/chika"
}

ARN is Amazon resource name

# AWS Billing 
Here's an explanation of what i learned about AWS billing, setting up budgets and alerts

AWS Billing: You learned about AWS billing, which refers to the charges incurred for using AWS services and resources. AWS provides several tools for managing your billing, such as the AWS Billing and Cost Management console, which allows you to view your usage, costs, and payment history.

Setting up Budgets and Alerts: You learned how to set up budgets and alerts in AWS to help manage your costs. Budgets allow you to set a spending limit and receive alerts when you approach or exceed that limit. Alerts can be configured to notify you via email or SMS when certain spending thresholds are reached.

# AWS organizations
AWS Organizations: You also learned about AWS Organizations, which is a service that allows you to centrally manage and govern multiple AWS accounts. With AWS Organizations, you can create groups of AWS accounts and apply policies to those groups, such as access controls and cost management policies. This allows you to manage your AWS resources more efficiently and effectively, especially if you have multiple accounts across different teams or business units.
