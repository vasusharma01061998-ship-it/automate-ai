# A-06 - Service Assurance Agent

## High Level Workflow

![Workflow](workflow.png)

**Flow:** START -> Ingest -> Router -> Radio / Transport / Core -> Planner -> Judge

- Judge will keep it in a loop until Confidence goes above 0.80
- After that, a Brief will be created for Human Review