# Week 2 — Distributed Tracing


## HOMEWORK/TECHNICAL TASKS
I instrumented the backend flask application to use Open Telemetry with Honeycomb.io as the provider

I then run queires to explore tarces with Honeycomb then instrument AWS X-Ray into backend flask application.

![Proof of Task]()

I provisioned X-Ray daemon within docker-compose and sent data back to X-Ray API then observed the traces within AWS Console
![Proof of my AWS Console]()

I also integrated Rollbar for Error Logging and triggered error logging.
Lastly I installed Watch Tower, wrote a custom logger to send application to Cloud Watch Log Group

## HOMEWORK CHALLENGES
- [x] Instrumenting Honeycomb for the frontend-application to observe network latency between frontend and backend

![Proof of task]()

- [x] Running custom queries in Honeycomb and save them later eg. Latency by UseID, Recent Traces.

![Proof of task]()
