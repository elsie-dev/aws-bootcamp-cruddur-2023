# Week 3 — Decentralized Authentication

## HOMEWORK/TECHNICAL TASKS

- I provisioned Amazon Cognito User Pool via ClickOps

![Proof of Task](assets/Week%203%20Cognito%20Userpool.JPG)
- I also implemented API calls to Amazon Cognito for custom login,sign up, recovery and forgot password ad adding a preffered Username

![Proof of task](assets/Week3%20adding%20preferred%20name.JPG)

I also verified JWT Token server side to serve authenticated API endpoints in Flask Application.

## ALTERNATIVES AND CONSIDERATIONS
- [x] Setup Azzure AD B2C solution. Since its low cost it supports many Identity Providers (IpDs)

## HOMEWORK CHALLENGES

- [x] Implemented MFA that sends code to my authentication app for me to be able to login into the application
- Added MFA device to elcymarion on AWS Console
![Proof of Task](assets/Week3%20MFA.JPG)
 - Installed the Authentication app to my mobile device , then scanned the QR Code, so every time you get a prompt and a verification code sent.
 
 -![Proof of Task](assets/Week%203%20MFA%20codeinput.JPG)

- [x] Decoupled the JWT verify process using Enovy as a sidecar
- Created envoy.yaml file 

![Proof of Task](assets/Week%203%20envoy%20file.JPG)

- Added the necessary envoy sidecar command to the app.py in the backend-flask folder
- Containerised the application, created Dockerfile then added necessary command to docker compose file.

- ![Proof of Task](assets/Week3%20envoy%20container.JPG)


## REFERENCE USED:
- Used [https://www.envoyproxy.io/](https://www.envoyproxy.io/docs/envoy/latest/start/docker) getting started with envoy
- To better understand Envoy containers used https://www.sobyte.net/post/2021-11/envoy-usage-demo/ for reference.
-  Used Chatgpt commands for deploying envoy in the backend flask application.


