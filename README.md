#CI/CD Pipeline for App Deployment
This Jenkins pipeline automates the build, test, and deployment process for your application.

Pipeline Overview
A declarative Jenkins pipeline that runs through three main stages: Build, Test, and Deploy, with success/failure notifications.

text
Build → Test → Deploy
Pipeline Stages
1. Build Stage
Builds the application

Outputs: "Building the app..." and "build completed"

2. Test Stage
Runs automated tests

Outputs: "Running tests..." and "testing completed"

3. Deploy Stage
Deploys to staging environment

Outputs: "Deploying to staging..." and "deploying completed"

Post-Build Actions
Status	Message
Success	"rizwana successfully deployed a ci cd pipeline!"
Failure	"oops! i messed pipeline"




<img width="1366" height="654" alt="2026-02-11" src="https://github.com/user-attachments/assets/efafdd41-1ba0-43ac-83aa-6567333f0fb5" />




Deployment Status
✅ Successfully deployed on Jenkins!


Created by: Rizwana
