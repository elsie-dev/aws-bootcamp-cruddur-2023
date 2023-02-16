# Week 0 — Billing and Architecture

## Homework Challenge
- [] Destroy your root account credentials, Set MFA, IAM role
- [] Use EventBridge to hookup Health Dashboard to SNS and send notification when there is a service health issue.
- [] Review all the questions of each pillars in the Well Architected Tool (No specialized lens)
- [] Create an architectural diagram (to the best of your ability) the CI/CD logical pipeline in Lucid Charts
- [] Research the technical and service limits of specific services and how they could impact the technical path for technical flexibility. 
- [] Open a support ticket and request a service limit




## TASK ACCOMPLISHED.
 ### Created Two budgets on AWS:
__One for ZeroSpend Budget__ - Notifies when my spending exceed areforecasted to exceed the free tier limit.

__Credit Limit Budget__ - Covers costs used in billings for the allowed resources.
For the two budgets included notification emails and action( stopping the EC2 when limit is exceeded)

Next is navigating to the project repo, then using the gitpod button we navigate to vscode. 
Installing AWS CLI
```curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
```

*Note:* While installing the AWS CLI ensure you check your current directory then move to the aws folder using **cd..** and this is where we install the  aws cli. __Reason__:(Installing it in the wrong place,with gitpod everything in the directpry gets committed.)

We also don't use **aws configure** instaed for the environment variables instead we use:
export AWS_ACCESSKEY, export AWS SECRET_ACCESS_KEY and export AWS_DEFAULT_REGION

To confirm identity we use ```aws sts get-caller-identity```

Next is Creating the AWS CLI Budget, https://docs.aws.amazon.com/cli/latest/reference/budgets/index.html


