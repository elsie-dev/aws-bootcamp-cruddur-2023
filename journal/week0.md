# Week 0 — Billing and Architecture

## REQUIRED HOMEWORKS/TASKS
- [x] Destroy your root account credentials, Set MFA, IAM role
- [x] Use EventBridge to hookup Health Dashboard to SNS and send notification when there is a service health issue.
- [x] Review all the questions of each pillars in the Well Architected Tool (No specialized lens)
- [x] Create an architectural diagram (to the best of your ability) the CI/CD logical pipeline in Lucid Charts
- [x] Research the technical and service limits of specific services and how they could impact the technical path for technical flexibility. 
- [x] Open a support ticket and request a service limit


 ### Created Two budgets on AWS:
 
__One for ZeroSpend Budget__ - Notifies when my spending exceed areforecasted to exceed the free tier limit.

__Credit Limit Budget__ - Covers costs used in billings for the allowed resources.
For the two budgets included notification emails and action( stopping the EC2 when limit is exceeded)

### Installing and Verifing AWS CLI:
I used Gitpod as instructed from the videos, and proof of work can be viewed fom my [gitpod.yaml file]().

**Proof of AWS CLI installation - ADD IMAGE.**

### AWS CLI Budgets:
I created AWS AWS Budget from the cli using commands from the youtube video.
Issue l run into while on the Gitpod
'' Parameter validation failed:
Invalid length for parameter AccountId, value: 9, valid min length: 12 '' - To solve this from stackoverflow turns out , l hadn't included my account ID the right way in the env terminal.

### Creating an SNS Topic
I created an SNS topic from the CLI then included the Billing Alarm as per the instructions
**proof of work** : 

### Creating a Budget
I created my own budget for to help with costs estimates.
![Billing Budget]()

![Billing Alarms]()

### Recreating the Logical Architecture Design
I succesfully recreated the Crudder Conceptual Diagram, and one of the unique feature, is the colour arrow between the Dynamo DB, Amazon RDS and Appsync this is because ..............

Here's the link to my [Lucid Diagram](![image](https://user-images.githubusercontent.com/62996370/219619577-7e6f945c-864d-46b8-b1b3-c9c6d819279c.png)
) and ![Screenshot image]() to show proof of work.

## HOMEWORK CHALLENEGS


## KEY TAKEAWAYS:
* While installing the AWS CLI on the Gitpod rem to __NOT__ use aws configure for the credential instaed use the export aws since this is an enviroment variable that we don't intend to be committed. 
* Also ensure you are in the right folder not inside the working directory for your crudder project
* Creating and Viewing Budgets might return an error from the user account, ensure to specify the billing policies to have access.
* Saving your AWS account ID, region, secret and access key to avoid starting afresh on gitpod everytime is highyl recommended.
* 
