# Project-4: Re-Architecting Web App on AWS Cloud[Cloud Native]

#### In project, I re-architected the web application in other to boost agility and improve business continuity so new features can be added easily for easy scalability and good performance.
For my front end:
#### ✔️ I used Elastic Beanstalk to deploy the application to Tomcat. EBS also created LoadBalancer, CloudWatch alarms, and Auto scaling groups for the app servers.
For my back end:
#### ✔️ MySQL instance was replaced with RDS MySQL.
#### ✔️ Memcached instance was replaced with Amazon ElastiCache service.
#### ✔️ RabbitMQ was replaced with Amazon MQ.
#### ✔️ CloudFront was created as content delivery network for the application.
### Flow:
#### The user is to access the URL which will, in turn, be resolved to an endpoint from Amazon route53, the endpoint will be of amazon cloudfront content delivery network which will cache a lot of stuff to serve the global audience. The request will be redirected to the application LB which is a part of the elastic beanstalk.
#### The application LB will then forward the request to an EC2 instance which is an ASG running our tomcat app service and this also will be part of our Elastic Beanstalk.
#### Cloudwatch alarms will be set to monitor autoscaling groups that will scale in and out if required.
#### Our artifact will be stored in an s3 bucket and the latest artifacts can be deployed with just a click.

#### Detailed steps:
#### https://medium.com/@osomudeyazudonu/project-4-re-architecting-web-app-on-aws-cloud-cloud-native-aac859ea2c04
