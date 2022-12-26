## For this project, I included continous delivery (CD) to my previous CI project "project 6" using just AWS services.

So basically,

🔨 Developers makes regular code commits that triggers our pipeline

🔨 Commit happens on AWS codebuild, triggering AWS codebuild

🔨 Codebuild does code analysis (sonar scanner)

🔨 Dependencies needed are downloaded from AWS codeartifact

🔨 Code build runs MAVEN to build artifact

🔨 Artifact is stored in an s3 bucket

🔨 "AWS deploy" deploys our artifact to beanstalk environment

🔨 Beanstalk will be connected to RDS

🔨 SoftWare Testing will be executed from AWS codebuild service which will come after our "Deploy" stage

## For This Project,

💊 I created Beanstalk And RDS

💊 Deployed DB in RDS

💊 Created a Deply Job for Beanstalk

💊 Created a Job Build to test our software

💊 Our output and snapshot was uploaded to s3 bucket

#### GitHub: https://lnkd.in/daeAaswY

#### Medium: https://lnkd.in/dUe4BSmp
