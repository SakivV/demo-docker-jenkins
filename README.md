# Demo-Docker-Jenkins

## Docker Hub Account Creation
1. Open Account on Dockerhub (https://hub.docker.com/). 
2. Once account is created, create Repo on docker hub.

## EC2 Instance Setup with Docker and Jenkins
1. Set up Jenkins on EC2 instance.
2. Install Docker on EC2 instance.
3. Install below plugin in Jenkins:
   1. docker
   2. docker-compose
   3. github

## Creating Jenkins Pipeline
1. Refer Jenkinsfile in this repo and as per that you can create your own. I would suggest try simple changes(single stage) for test purpose.
2. In Jenkins, create New item/job -> Select Pipeline.
3. Enter necessary details:
   1. Select PollSCM to trigger pipeline on push.
   2. Github repo URL
   3. In Pipeline section, select option Pipeline from SCM as our pipeline code is in repo. 
   4. Enter your github repo URL.
   5. Once doen , click save.

## Run pipeline
1. Run pipelein manually for test. You can do this by using Build Now option.
2. Make changes in project and push changes to repo, check pipeline is getting triggered automatically.