## FLOW

- User will access website by using url and that url will be pointed to an endpoint in name cheap dns
- Users browser will use the endpoint to connect to Load balancer by using https.
- The certificate for https encryption will be mentioned in ACM
- User will access applications load balancer endpoint
- Load balancer will be in a security group and will only allow our HTTPs traffic
- applications load balancer will route the request to Apache Tomcat service instances being managed by auto scaling group.
- As per high or low load these instance capacity will scaled out or stalled in…
- Tomcat ec2 instance will be in a separate sg and will only allow traffic on port 8080 only from LB
- Information of Backend services or server IP add (MYSQL, RabbitMQ, Memcache) will be mentioned in a route53 private DNS zone so Tomcat instances will access back server with a name mentioned in which will be mentioned in Route 53 private DNS where the private IP add of our backend servers will be mentioned.
- The backend services will be mentioned in separate sg 
