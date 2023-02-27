# Week 0 — Billing and Architecture

## REQUIRED HOMEWORK/TASKS
These are some of the techical tasks l completed for these week.

 ### Created Two budgets on AWS:
 
__ZeroSpend Budget__ - Notifies when my spending exceed areforecasted to exceed the free tier limit.

__Credit Limit Budget__ - Covers costs used in billings for the allowed resources.
For the two budgets included notification emails and action( stopping the EC2 when limit is exceeded)

### Installed and Verified AWS CLI:
I used Gitpod as instructed from the videos,proof of work can be viewed fom my [gitpod.yaml file]().

**Issue faced while commiting my changes:** 
*You have diveregent branches and need to specify how to reconcile them* 
- *Solved this* with the help [GitHub Issues](https://github.com/desktop/desktop/issues/14431)


![Proof of working AWS CLI](assets/Week%200%20AWS%20CLI.JPG)

### AWS CLI Budgets:
I created AWS Budget from the cli using commands from the youtube video.

**Issue faced while on the Gitpod:**
*Parameter validation failed:
Invalid length for parameter AccountId, value: 9, valid min length: 12*
- *Soved this* through [stackoverflow](https://stackoverflow.com/questions/59822733/please-solve-the-error-in-aws-cli-parameter-validation-failed) which turns out , l hadn't included my account ID the right way in the env terminal and was returned empty value while tring to create the budget.

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
I recreated the Conceptual Diagram but added private and public subnets on both my frontend and backend and a NAT Gateway.
(Explaining further in the Homework Challenge)

In addition to that you can notice the arrows from Amazon Dynamo DB and RDS to App sync are different, since Appsync contains resolvers used to read and write dat from the two Databases.

![Cruddur Logical Design](assets/Logical%20Diagram.JPG)
 Additional proof of the [Lucid Share Link](https://lucid.app/lucidchart/cd84a441-e50e-4431-8e92-805aa20150c9/edit?viewport_loc=-1256%2C506%2C4302%2C1581%2C0_0&invitationId=inv_04a6dcf8-425a-4ef7-a14b-97a52e6046cc)


## HOMEWORK CHALLENGES
- [x] Additional icons in the Logical Diagram
 - Since security is essential in the Cruddur Application, l intend to restict netwrok traffic to my database by allowing only legitimate traffic to reduce attacks.
 - The databases at the backend are secured in the private subnet so as to not access internet directly.
 -  However the database servers can send and receive internet traffic through the NAT device in the public subnet located at the frontend.

- [x] Conceptual CI/CD Diagram 
- I designed this to indicate possible automations from code builds to code deploying from Github.
- With CICD work can be carried out faster and with minimal human errors. In addition small bug fixes can easily be noticed.

 [CICD Design](https://lucid.app/lucidchart/9a3aa242-6532-488f-804c-161b73238eef/edit?view_items=HllynDte0Wk7&invitationId=inv_d9c8df5f-4720-46f2-9da7-346ef8369540)
 
- [x] Review all the questions of each pillars in the Well Architected Tool (No specialized lens)
** TO BE ADDED SOON*
### Reference for the Homework Challenges

**TO BE ADDED SOON**


## KEY TAKEAWAYS:
* While installing the AWS CLI on the Gitpod rem to __NOT__ use aws configure for the credential instaed use the export aws since this is an enviroment variable that we don't intend to be committed. 
* Also ensure you are in the right folder not inside the working directory for your crudder project
* Creating and Viewing Budgets might return an error from the user account, ensure to specify the billing policies to have access.
* Saving your AWS account ID, region, secret and access key to avoid starting afresh on gitpod everytime is highyl recommended.

