# Week 0 — Billing and Architecture

## REQUIRED HOMEWORKS/TASKS
These are some of the techical tasks l completed for these week.

 ### Created Two budgets on AWS:
 
__ZeroSpend Budget__ - Notifies when my spending exceed areforecasted to exceed the free tier limit.

__Credit Limit Budget__ - Covers costs used in billings for the allowed resources.
For the two budgets included notification emails and action( stopping the EC2 when limit is exceeded)

### Installed and Verified AWS CLI:
I used Gitpod as instructed from the videos, and proof of work can be viewed fom my [gitpod.yaml file]().

![Proof of working AWS CLI](assets/Week%200%20AWS%20CLI.JPG)

### AWS CLI Budgets:
I created AWS Budget from the cli using commands from the youtube video.
Issue l run into while on the Gitpod
*Parameter validation failed:
Invalid length for parameter AccountId, value: 9, valid min length: 12*
- Soved this through [stackoverflow](https://stackoverflow.com/questions/59822733/please-solve-the-error-in-aws-cli-parameter-validation-failed) which turns out , l hadn't included my account ID the right way in the env terminal and was returned empty value while tring to create the budget.

### Created a Budget
I created my own budget for to help with costs estimates.
![Proof of Billing Budget](assets/week0%20budgets.JPG)

### Creeated Billing Alarm
I also created a billing laarm to help with daily estimated charges and get an email notification whenever the charge is about to be exceeded.
![Proof of Billing Alarm](assets/Billing%20Alarm.JPG)

### Created an SNS Topic
I created an SNS topic from the CLI then included the Billing Alarm as per the instructions
![Proof of SNS Topic](assets/Week%200%20SNS%20Topic.JPG)


### Recreated the Logical Architecture Design
I succesfully recreated the Crudder Conceptual Diagram, and one of the unique feature, is the colour arrow between the Dynamo DB, Amazon RDS and Appsync this is because ..............

![Cruddur Logical Design](assets/lucid%20architecture.JPG)
 Additional proof of the [Lucid Share Link](https://lucid.app/lucidchart/cd84a441-e50e-4431-8e92-805aa20150c9/edit?page=0_0#)


## HOMEWORK CHALLENEGS
- [x] Review all the questions of each pillars in the Well Architected Tool (No specialized lens)
- [x] Research the technical and service limits of specific services and how they could impact the technical path for technical flexibility. 
- [x] Open a support ticket and request a service limit

### Reference challenges

## KEY TAKEAWAYS:
* While installing the AWS CLI on the Gitpod rem to __NOT__ use aws configure for the credential instaed use the export aws since this is an enviroment variable that we don't intend to be committed. 
* Also ensure you are in the right folder not inside the working directory for your crudder project
* Creating and Viewing Budgets might return an error from the user account, ensure to specify the billing policies to have access.
* Saving your AWS account ID, region, secret and access key to avoid starting afresh on gitpod everytime is highyl recommended.

