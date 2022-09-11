# Cloud_Journey
Creating_Budgets_with_AWS
AWS BUDGET

Budgets are set to notify or alarm you on your billings whiles you use AWS.
 It provides statistics on which services take up the most  and least cost and at which time. 
 
To do this, 
    • first log in into your AWS console as a root user.
    • Go to AWS cost explorer and click on it, it opens up cost management
    • On the left side, click budget. Then create budget.
    • On cost budget, select next to name the budget. 
    • Scroll down to input name preference e.g weekly budget
    • Scroll down to enter budget amount e.g 1$
    • Set incident respone to everything then click next
    • Configure threshold and set a percentage for that. Preferrably 80%
    • Add your receipient email for notification. Click next
    • Confirm budget and choose create.
    • Budget created, download your CSV before closing the window down.



Creating IAM users and groups, Adding MFA And Attaching policies.

Identity and access management(IAM) is a services in AWS used to grant permissions to different users and group depending on their assigned roles and responsibility within an organisation. You can configure MFA to users and attach policies as you practice best practices to secure organisation.

Steps to follow to create user and attaching policies
    • Log into the AWS management console
    • Under all services, Select IAM.
    • On the lest side of the dash board, select users
    • Select add user
    • Input the users name and add preferred credential type to allocate to the user. Either choosing Access Key or Password or both.
    • Select a password type to use. With custom password, you choose the password the user would use.
    • Unable the require password reset option to allow user to conform to just the password allocated.
    • Click next to add permisson whether to add a user to  group ,attach policies or copy permissions that already exist.
    • Select attach policies. You can either create policies or attach already existing policies that fit the organisations standard. Choose ec2 and s3 full access policy.
    • You can add tags for easy identification or skip and choose next if you do not want it to review.
    • Review your policies and other user details to move forward.
    • Create user. Download the .csv before closing the window because it contains the link for user access but not the password. Password is only known by the organisation.

Creating Groups

Groups are created for easy management and organisation. Each user added to a group inherits the policies assigned to the group.

let’s see how this is done:
    • In the IAM console, Go to user group and select create group
    • Name the group 
    • You can select which user should be in the group and also attach policies. Not compulsory though.
    • Select create group when done

Settting MFA

    • Select user
    • Then security credentials
    • Follow the next instructions to set up virtual MFA on device