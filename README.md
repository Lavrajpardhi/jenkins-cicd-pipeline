# Jenkins CI/CD Pipeline – DevOps Task 2

## Objective

Create a simple Jenkins CI/CD pipeline to automate the build, test, and deployment process of a Node.js application.

## Tools Used

* Jenkins
* GitHub
* Git
* Node.js
* npm

## Project Structure

```text
jenkins-cicd-pipeline/
├── app.js
├── package.json
└── Jenkinsfile
```

## Jenkins Pipeline Stages

### 1. Build

Installs the required Node.js dependencies using:

```bash
npm install
```

### 2. Test

Checks the Node.js application using:

```bash
npm test
```

### 3. Deploy

Runs the deployment step through the Jenkins pipeline.

## CI/CD Flow

```text
Developer
    ↓
GitHub Repository
    ↓
Jenkins
    ↓
Build
    ↓
Test
    ↓
Deploy
    ↓
Successful Pipeline
```

## Automatic Trigger

Jenkins is configured with **Poll SCM** to check the GitHub repository for new commits.

When a new commit is detected, Jenkins automatically starts the pipeline.

## Result

The Jenkins pipeline was successfully tested with:

* Build: SUCCESS
* Test: SUCCESS
* Deploy: SUCCESS
* Automatic trigger: SUCCESS

The pipeline completed successfully with:

```text
Finished: SUCCESS
```
