# Project-10: Continuous Delivery & Configuration Management (Jenkins&Ansible)

[_Project Source_](https://www.udemy.com/course/devopsprojects/?src=sac&kw=devops+projects)

#####
Starting the new year with Ansible,

but before I liter your timeline with my projects.

I want to say a Happy New Year Guys!!.

Curently, I have been learning ansible and on this project I combined the power of Jenkins and Ansible in extension to my prevoius CI project "Project 5", using ansible to stage and deploy the pipeline to production environment.

🩸 Developer makes code changes, which is detected by Jenkins and fetches all changes made.

🩸 Jenkins runs code/unit test and if passed or failed sends a notification to slack, but if passed continues on the next job which is code analysis using checkstyle and sonarqube scanner and the report forwarded to our sonarqube server.

🩸 Sonarqube server compares this result with quality gates abd if passed next job gets triggered with MAVEN building our artifact and dependencies downloaded from our nexus repo.

🩸 Artifact gets packaged and uploaded to nexus repo if passed.

🩸 ANSIBLE downloads the artifact from nexus and deploys it to our staging environment while making sure the right packages and services are installed.

🩸 Ansible will roll back to its previous state if the the stage fails.

🩸 If passed and done, sofware testing and DevQ gets executed.

🩸 If approved, Ansible is used to deploy the artifact to our production server.

#####

#### See detailed practical steps here: https://medium.com/@osomudeyazudonu/continuous-delivery-configuration-management-using-jenkins-ansible-ce38030cdae9

####GitHub: https://github.com/Osomudeya
