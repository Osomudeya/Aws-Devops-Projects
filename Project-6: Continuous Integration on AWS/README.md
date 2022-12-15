# Project-6: Continuous Integration on AWS Cloud

In this DevOps project, I set up continuous integration pipeline using AWS managed services.

⬆️ When developer makes code change and commits to the repo in AWS CodeCommit CodePipeline will be triggered:
🏃🏼‍♂️ Latest source code is fetched from the repo
✅ CodeBuild job will run SonarCloud analysis and check quality gates
⬇️ Download dependencies from CodeArtifact
🗿 If completed successfully, the build job generates artifact
🪣 Resulting artifact is stored in S3 bucket
📨 SNS notification sent with Pipeline status

In the next project, this pipeline will be extended to include continuous delivery.

[_Project Source_](https://www.udemy.com/course/devopsprojects/?src=sac&kw=devops+projects)

## Project Documemtation:

https://medium.com/@osomudeyazudonu/project-6-continuous-integration-on-aws-cloud-a3e2dd199b
