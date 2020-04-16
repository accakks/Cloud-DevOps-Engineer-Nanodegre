# Lesson 1: Getting Started With [CloudFormation](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/Welcome.html)

- The **IaaS** allows a user to provision Virtual Machines (VMs), set up networks (VPC), create subnets, and associate necessary security features. Further, VMs can be attached to storage volumes, different networks, or servers. All the resources mentioned above are referred to as **Infrastructure**.

![](https://drive.google.com/file/d/18U_uH-LaZ1qmQqusClgC7zE1BEOM4KSa/view?usp=sharing)

- **CloudFormation**: CloudFormation is a tool in AWS for managing, configuring and deploying infrastructure (push code along with the necessary server configurations).
- CloudFormation is a declarative language, not an imperative language.
- CloudFormation handles resource dependencies so that you don’t have to specify which resource to start up before another.


#### DevOps
- A set of practices that works to automate and integrate the processes between software development and IT teams, so they can build, test, and release software faster and more reliably.
- Development + Operations
- Issues that DevOps tries to solve:
	- Unpredictable deployments
	- Mismatched environments (development doesn’t match production)
	- Configuration Drift
- One of the benefits of using DevOps is that it allows _predictable_ deployments using _automated_scripts.
- [DevOps tools vs. Software Configuration Tools.](https://softwareengineering.stackexchange.com/questions/130850/difference-between-devops-and-software-configuration-management)
![DevOps](https://i.stack.imgur.com/kEOe7.png)

- The most important DevOps practices are:
	-[**Continuous Integration / Continuous Delivery (CI/CD)** ](https://www.atlassian.com/continuous-delivery/principles/continuous-integration-vs-delivery-vs-deployment) : Continuous integration is the process flow of testing any change made to your development flow, while continuous deployment tracks those changes through to staging and production systems. Example tool: Jenkins, CircleCI. 
	- [**Infrastructure as Code (IaaC)**](https://en.wikipedia.org/wiki/Infrastructure_as_code) - configuration and management of cloud infrastructure using re-usable scripts.
	Other prevalent practices are:
	- Microservices
	- Monitoring and Logging
	- Communication and Collaboration


#### Setting up tools for CloudFormation
- Set up IAM (Identity and Access management) user and select Access.
- Install AWS CLI
TIP: Make a key inactive instead of deleting (for example when you wanna pause an automated process that uses that key. 

_Write a CloudFormation Script (can use YML or JSON)_
_Create a CloudFormation Stack (can also write a shell script) using create-stack or update-stack to update existing stack_
_See if it worked/created in console_

_manual vs. automated provisioning of EC2 instances in a VPC_