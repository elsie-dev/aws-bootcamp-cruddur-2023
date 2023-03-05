# Week 2 — Distributed Tracing
For week two task l have been having a problem with my GitPod Workspace and, therefore shifted to using GitHub Codespace. 
For managing env variables for Honeycomb,I secured them under my Gthub Secrets and then restarted my codespace.

## HOMEWORK/TECHNICAL TASKS

I instrumented the backend flask application to use Open Telemetry with Honeycomb.io as the provider

I then run queires to explore traces with Honeycomb then instrument AWS X-Ray into backend flask application.

![Proof of Honey comb](assets/Week%202%20Honeycomb%20traces.JPG)

Configuring X-ay daemon within docker-compose to send data to X-Ray API

![](assets/CaptureWeek2%20sending%20data%20back%20to%20X-RAY%20API.JPG)

I provisioned X-Ray daemon within docker-compose and sent data back to X-Ray API then observed the traces within AWS Console

![Proof of traces on AWS Console](assets/Week2%20tracefromxray.JPG)

 I also installed Watch Tower, wrote a custom logger to send application to Cloud Watch Log Group.
 
 ![](assets/Week2%20cloudwatch%20traces%20terminal.JPG )

Lastly l integrated Rollbar for Error Logging and triggered error logging.

![Rollbar Console]()

## HOMEWORK CHALLENGES
- [x] Instrumenting Honeycomb for the frontend-application to observe network latency between frontend and backend

![Proof of task]()

- [x] Running custom queries in Honeycomb and save them later eg. Latency by UseID, Recent Traces.

![Proof of task]()

### ISSUES ENCOUNTERED:
Getting 502 gateway when running the ports from Codespaces. Solution, changing port protocal to either HTTP or HTTPS and restarting the terminal.
[Stackoverflow](https://github.com/community/community/discussions/285630)
