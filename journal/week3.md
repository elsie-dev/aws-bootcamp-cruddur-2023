# Week 3 — Decentralized Authentication

## HOMEWORK/TECHNICAL TASKS
- Provisioning Amazon Cognito User Pool
-
- Im plementing API calls to Amazon Cognito for custom login,sign up, recovery and forgot password

![Proof of task]()



### HOMEWORK CHALLENGES
[X] Implemented MFA that sends code to my authentication app for me to be able to login into the application
- Added MFA device to elcymarion on AWS Console
![Proof of Task]()
 - Installed the Authentication app to my mobile device , then scanned the QR Code, so every time you get a prompt and a verification code sent.
 -![Proof of Task]()

[X] Decoupled the JWT verify process using Enovy as a sidecar
- Created envoy.yaml file 
![Proof of Task]()
- Added the necessary envoy sidecar command to the app.py in the backend-flask folder
- Containerised the application, created Dockerfile then added necessary command to docker compose file.
- ![Proof of Task]()

## REFERENCE USED:
- Used [https://www.envoyproxy.io/](https://www.envoyproxy.io/docs/envoy/latest/start/docker) getting started with envoy
- To better understand Envoy containers used https://www.sobyte.net/post/2021-11/envoy-usage-demo/ for reference.
-  Used Chatgpt commands for deploying envoy in the backend flask application.


