### Infrastructure as Code
  - [Sample CloudFormation templates for ECS](https://github.com/awslabs/aws-cloudformation-templates/tree/master/aws/services/ECS) - Examples of launching containers with both public, and private networking, behind a public facing load balancer, as well as behind a private, internal load balancer.
  - [CloudFormation ECS](https://github.com/awslabs/ecs-refarch-cloudformation) - Reference architecture for deploying microservices to ECS in tiered VPC with NAT gateways and two availability zones.
  - [Terraform ECS](https://github.com/arminc/terraform-ecs) by [Armin Coralic](https://twitter.com/acoralic) - Production ready AWS ECS infrastructure as code with Terraform
  - [CloudFormation Templates by Cloudonaut](https://cloudonaut.io/new-cloudformation-templates-ecs-cluster-service-legacy-vpc-wrapper-automated-tests/)

### Implementation Guides

Examples of how to do advanced customizations on your ECS cluster:

  * __Autoscaling__
    - [Autoscaling services in ECS](https://www.codementor.io/jholub/amazon-ecs-auto-scale-docker-containers-6keydo24n) - How to autoscale the number of service tasks
    - [Autoscaling the cluster in ECS](http://garbe.io/blog/2016/10/17/docker-on-ecs-scale-your-ecs-cluster-automatically/) - How to autoscale the number of EC2 instances in a cluster
    - [Advanced ECS cluster autoscaling](http://garbe.io/blog/2017/04/12/a-better-solution-to-ecs-autoscaling/) - A more advanced technique for autoscaling an ECS cluster, with more effective scale in as well as out
    - [Lambda based approach for cluster scale-in](https://github.com/omerxx/ecscale)
    - [Extending ECS autoscaling for under $2 a month with Lambda](https://www.miketheman.net/2017/01/09/extending-ecs-auto-scaling-for-under-2month-with-lambda/)
    - [Scale in script in Python](https://medium.com/@dinushad92/scale-down-ec2-container-instances-in-ecs-fb97f895ac9c)
  * __Networking__
    - [Private subnets tutorial](https://www.topcoder.com/blog/aws-container-services-private-subnets-tutorial/)
    - [End-to-end TLS traffic](https://aws.amazon.com/blogs/compute/maintaining-transport-layer-security-all-the-way-to-your-container-using-the-network-load-balancer-with-amazon-ecs/) - How to setup end-to-end TLS from client to container, as well as from container to container
  * __Service Discovery__
    - [Using DNS](https://github.com/awslabs/ecs-refarch-service-discovery/)
  * __Data Persistance__
    - [Using Amazon Elastic File System](https://aws.amazon.com/blogs/compute/using-amazon-efs-to-persist-data-from-amazon-ecs-containers/)
  * __Secrets Management__
    - [Using Parameter Store and IAM Roles for Tasks](https://aws.amazon.com/blogs/compute/managing-secrets-for-amazon-ecs-applications-using-parameter-store-and-iam-roles-for-tasks/)
    - [Using ECS Task roles for managing AWS credentials](https://medium.com/@RemindEng/keeping-aws-secrets-secret-with-ecs-ec4a51517b4d)
    - [The right way to store secrets using Parameter Store](https://aws.amazon.com/blogs/mt/the-right-way-to-store-secrets-using-parameter-store/)
  * __Administration__
    - [Automatically draining cluster instances before termination](https://aws.amazon.com/blogs/compute/how-to-automate-container-instance-draining-in-amazon-ecs/)
    - [Monitor cluster state with Cloudwatch event stream](https://aws.amazon.com/blogs/compute/monitor-cluster-state-with-amazon-ecs-event-stream/)
    - [Run an ECS Task on every cluster instance](https://aws.amazon.com/blogs/compute/running-an-amazon-ecs-task-on-every-instance/)


### Open Source
  - [docker-elk-ecs](https://github.com/markriggins/docker-elk-ecs) - Connecting Amazon ECS container logs to an ELK (Elasticsearch, Logstash, Kibana) stack

### Reference Architectures
  - [Microservice cloudformation stack](https://github.com/awslabs/ecs-refarch-cloudformation)
  - [Sock shop microservices demo on Amazon ECS](https://github.com/microservices-demo/microservices-demo)
  - [Node.js Microservices](https://github.com/awslabs/amazon-ecs-nodejs-microservices)
  - [Java Microservices on AWS ECS](https://github.com/awslabs/amazon-ecs-java-microservices)
  - [Swift ECS Workshop](https://github.com/awslabs/swift-ecs-workshop)
  - [NGINX Reverse Proxy sidecar container on AWS ECS](https://github.com/awslabs/ecs-nginx-reverse-proxy)
  - [Deploying a Deep Learning Framework on ECS](https://github.com/awslabs/ecs-deep-learning-workshop)
  - [Powering your Amazon ECS Cluster with Amazon EC2 Spot Instances](https://github.com/awslabs/ec2-spot-labs/tree/master/ecs-ec2-spot-fleet)
  - [Cats n' Dogs](https://github.com/aws-samples/amazon-ecs-catsndogs-workshop) - A fun workshop that covers service and container-instance auto-scaling, spot-fleet integration, container placement strategies, service discovery, secrets management with AWS Systems Manager Parameter Store, among other things.

### Continuous Integration / Continuous Deployment
  * __CI/CD using:__
    - [AWS CodePipeline](https://github.com/awslabs/ecs-refarch-continuous-deployment)
    - [Lambda](https://medium.com/@YadavPrakshi/automate-zero-downtime-deployment-with-amazon-ecs-and-lambda-c4e49953273d)
  * __CI/CD mechanics:__
    - [Rolling blue/green deploy in place](https://blog.codeship.com/easy-blue-green-deployments-on-amazon-ec2-container-service/)
    - [Isolated Regression Testing](https://aws.amazon.com/blogs/compute/amazon-ecs-at-the-climate-corporation-using-ecr-and-multiple-accounts-for-isolated-regression-testing/)

### Presentations
  - [Running your Dockerized application(s) on AWS EC2 Container Service](https://speakerdeck.com/mpas/running-your-dockerized-application-s-on-aws-ec2-container-service) by [Marco Pas](https://twitter.com/marcopas)
  - [Microservices on AWS with Weaveworks](https://www.youtube.com/watch?v=nSvpjZkmYIM)
  - [Running a Virtual World via ECS](https://www.youtube.com/watch?v=wGg_4aFOHsY) - Linden Labs on their usage of ECS
  - [Advanced Task Scheduling with AWS ECS](https://www.youtube.com/watch?v=RJZU0zZoKR8)
  - [Instacart on running microservices on Amazon ECS](https://www.youtube.com/watch?v=CtALTTjy7Qw)
  - [Building Next-Generation Applications with Amazon ECS](https://www.youtube.com/watch?v=xIc3WT6kAVw) - How Meteor Built Galaxy on Amazon ECS
  - [Amazon ECS at Coursera: A General Purpose Microservice](https://www.slideshare.net/AmazonWebServices/cmp406-amazon-ecs-at-coursera-a-generalpurpose-microservice)

### Tech Blogs

   - [Segment](https://segment.com) - [Rebuilding Our Infrastructure with Docker, ECS, and Terraform](https://segment.com/blog/rebuilding-our-infrastructure/)
   - [Docker on AWS: from containerization to orchestration](http://mherman.org/blog/2017/11/16/docker-on-aws-from-containerization-to-orchestration)

### Courses

  - [ECS Workshop using AWS Fargate and Mu](https://ecsworkshop.com/) - Learn how to deploy a 3 tier, polyglot, microservice based application to AWS Fargate for ECS using the Mu framework!
