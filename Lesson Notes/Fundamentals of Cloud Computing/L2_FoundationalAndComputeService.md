# Lesson 2: Foundational And Computer Service

#### [Elastic Cloud Compute - EC2](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/concepts.html)
- Provides server for rent (Instances) 
- Actual physical servers in an Accessibility Zone (Not Serverless)
- under the Compute section of the AWS Management Console.
Tip: Spot instances can save you up to 90% off the on-demand pricing.

#### [Elastic Block Store - EBS](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AmazonEBS.html)
- Storage solution for EC2 instances. Physical hardrive connected to server to increase storage. 
- EC2 has two types of memories: 
	- In memory(instance store)
	- EBS - [X] Able to persist data after EC2 is terminated. 
- Automatically replicated in AZ. 

#### [Virtual Private Cloud - VPC](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)
- Virtual private cloud allows you to create your own private network/space in cloud. Services can be launched inside it. 
- Allows controlling virtual networking environment: IP address ranges, creating public or private subnets, route tables, network gateways etc. 
- VPC lives within a region, can span across AZs. 
-  Found under Networking & Content Delivery section
- No addtional charges for VPC. 

*_Try accessing VPC, and launch an EC2 instance on it. Also attach an EBS volume_*

#### [Lambda - Computer power in cloud](https://aws.amazon.com/lambda/)
- Provides you with computing power in the cloud by allowing you to execute code without standing up or managing servers.
- Meant to do one specific task. The code you run on AWS Lambda is called a “Lambda function.” 
- Time limit: 15 mins. 
- Application dev using Lambda is Serverless.
- Event driven code. 
- Once code is uploaded(or authored via console), env takes care of everything needed to run or scale code. 
- Under the Compute section on the AWS Management Console.
- AWS Lambda supports Java, Go, PowerShell, Node.js, C#/.NET, Python, and Ruby. There is a Runtime API that allows you to use other programming languages to author your functions.


*_Create and Execute a lambda_*

#### [Elastic Beanstack](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/Welcome.html)
- An orchestration service that allows you to deploy a web application at the touch of a button by spinning up (or provisioning) all of the services that you need to run your application. (Automates the process)
- VPC, EC2 instance, Elastic load balancer automatically launched. 
- Can be used to deploy web applications developed with Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker.
- Under Compute section.
