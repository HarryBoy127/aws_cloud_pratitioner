#### What is Cloud Computing?
Cloud computing is the on-demand delivery of IT resources over the internet with pay-as-you-go pricing. On-demand delivery indicates that AWS has the resources you need, when you need them. 

#### What are the three deployment models for cloud computing, their definitions, and uses?
- Cloud-based Deployment Model, you can migrate existing applications to the cloud, or you can design and build new applications in the cloud. You can build those applications on low-level infrastructure that requires your IT staff to manage them.
  - Run all parts of the application in the cloud.
  - Migrate existing applications to the cloud.
  - Design and build new applications in the cloud.
- On-premises deployment is also known as a private cloud deployment.  In this model, resources are deployed on premises by using virtualization and resource management tools.
- Deploy resources by using virtualization and resource management tools.
  - Increase resource utilization by using application management and virtualization technologies.
- Hybrid deployment, cloud-based resources are connected to on-premises infrastructure. You might want to use this approach in a number of situations. For example, you have legacy applications that are better maintained on premises, or government regulations require your business to keep certain records on premises.
  - Connect cloud-based resources to on-premises infrastructure.
  - Integrate cloud-based resources with legacy IT applications.

  #### What are the Benefits of cloud computing and their definitions?
  - Scalability and flexibility
Cloud computing gives your business more flexibility. You can quickly scale resources and storage up to meet business demands without having to invest in physical infrastructure.
- Data loss prevention
Cloud providers offer backup and disaster recovery features. Storing data in the cloud rather than locally can help prevent data loss in the event of an emergency
- Advanced security
Despite popular perceptions, cloud computing can actually strengthen your security posture because of the depth and breadth of security features, automatic maintenance, and centralized management.

- Better collaboration
Cloud storage enables you to make data available anywhere you are, anytime you need it. Instead of being tied to a location or specific device, people can access data from anywhere in the world from any device—as long as they have an internet connection.
### What are the Amazon EC2 instance types and their definitions?
Amazon EC2 provides a wide selection of instance types optimized to fit different use cases. Instance types comprise varying combinations of CPU, memory, storage, and networking capacity and give you the flexibility to choose the appropriate mix of resources for your applications. Each instance type includes one or more instance sizes, allowing you to scale your resources to the requirements of your target workload.

### What is a Load Balancer?
A load balancer is a solution that acts as a traffic proxy and distributes network or application traffic across endpoints on a number of servers. 

### What is the primary purpose of AWS Regions in the global infrastructure?
The AWS Global Infrastructure is built for performance. AWS Regions offer low latency, low packet loss, and high overall network quality.


### Describe the function of Amazon CloudFront in AWS's architecture.
CloudFront speeds up the distribution of your content by routing each user request through the AWS backbone network to the edge location that can best serve your content.

### How do AWS Edge locations enhance the performance of Amazon CloudFront?

i) Reduced Latency: Edge locations are strategically placed in major cities around the world, bringing content closer to the end-users. 

ii) Caching Content: Edge locations cache copies of your content, such as images, videos, and other static files. When a user requests content, CloudFront serves it from the nearest edge location, avoiding the need to fetch it from the origin server.

### Explain how Amazon Route 53 integrates with AWS Edge locations to enhance user experiences.

Amazon Route 53 is a highly scalable and reliable Domain Name System (DNS) web service designed to route end-user requests to various AWS services, including AWS Edge locations, to enhance user experiences. Here's how Route 53 integrates with AWS Edge locations:

Global Traffic Management:

Latency-Based Routing: Route 53 can direct user requests to the AWS Edge location that provides the lowest latency, ensuring that users access the nearest and fastest edge location. This reduces load times and improves the overall user experience.
Geolocation Routing: Route 53 can route traffic based on the geographic location of users. This ensures that requests are handled by the nearest edge location, providing localized content and reducing latency.

### What are the four main factors to consider when choosing an AWS Region?
i) Latency, 
ii) price, 
iii) service availability, 
iv)  compliance

### What is an AWS Availability Zone?
Availability Zones consist of one or more discrete data centers, each with redundant power, networking, and connectivity, and housed in separate facilities.

### What is the purpose of having multiple Availability Zones within an AWS Region

Having multiple Availability Zones (AZs) within an AWS Region enhances the availability, reliability, and fault tolerance of applications. By distributing resources across AZs, you achieve redundancy, automatic failover, and disaster recovery, ensuring minimal downtime during outages. This setup also optimizes scalability, load balancing, and cost efficiency while meeting regulatory compliance and enhancing security.

### Why is it important to run EC2 instances across multiple AZs?

Running EC2 instances across multiple Availability Zones (AZs) is crucial for several reasons:

High Availability: Distributing EC2 instances across multiple AZs ensures that your application remains available even if one AZ experiences an outage or failure. This redundancy minimizes downtime and enhances the reliability of your services.

Fault Tolerance: Multiple AZs provide isolation from failures, such as power outages, hardware issues, or natural disasters, that may affect a single AZ. By spreading instances across AZs, you can maintain service continuity in the event of localized failures.

Improved Performance: Load balancing across multiple AZs can distribute traffic more evenly, preventing any single AZ from becoming a bottleneck. This improves the overall performance and responsiveness of your application.

### What are edge locations in AWS?
AWS Edge Locations are strategically positioned points in the AWS network optimized for low-latency content delivery, ensuring that data reaches users swiftly.

### What is AWS Outposts?
AWS Outpost is a pool of AWS compute and storage capacity deployed at a customer site

### How do Availability Zones within AWS Regions contribute to disaster recovery and high availability?

Availability Zones (AZs) within AWS Regions contribute significantly to disaster recovery and high availability by:

Redundancy: By distributing resources across multiple AZs, you ensure that an outage in one AZ does not affect your entire application, maintaining continuous availability.
Fault Isolation: Each AZ operates independently with separate power, cooling, and networking, so failures are contained and do not spread to other AZs.
Disaster Recovery: In the event of a natural disaster or significant failure in one AZ, resources in other AZs can take over, ensuring data and application continuity.
Load Balancing: Traffic can be distributed across AZs, preventing any single AZ from becoming overwhelmed and ensuring better performance and reliability.

### What is an API in the context of AWS?
In the context of AWS, an API (Application Programming Interface) is a set of protocols and tools that allows developers to interact with AWS services programmatically. APIs enable you to automate tasks, manage resources, and integrate AWS services with other applications and systems.

### What is the primary method of interacting with AWS services?
One of the most accessible and user-friendly ways to interact with your AWS resources is through the AWS Management Console. This web-based interface provides an intuitive and visual approach to managing your cloud infrastructure.
### What are the main ways to interact with AWS services?
The main ways to interact with AWS services are:

AWS Management Console: A web-based user interface that allows you to manage and monitor AWS services visually. It's user-friendly and suitable for users who prefer a graphical interface for configuring and managing their AWS resources.

AWS Command Line Interface (CLI): A tool that provides a set of commands for interacting with AWS services from a terminal or command prompt. It's ideal for automation, scripting, and managing resources programmatically.

AWS SDKs (Software Development Kits): These are available for various programming languages (such as Python, Java, JavaScript, .NET, and Ruby) and allow developers to interact with AWS services within their applications. SDKs simplify the process of making API calls and handling responses.

AWS APIs (Application Programming Interfaces): RESTful APIs that enable direct interaction with AWS services over HTTP. APIs are used for automation, integration with other services, and for creating custom solutions.

AWS CloudFormation: A service that allows you to define and provision AWS infrastructure as code using templates. This approach enables you to automate the setup and configuration of resources in a consistent and repeatable manner.

AWS CDK (Cloud Development Kit): An open-source software development framework that allows you to define cloud infrastructure using familiar programming languages. It leverages the power of programming constructs to manage AWS resources.

AWS Elastic Beanstalk: A platform-as-a-service (PaaS) offering that allows you to deploy and manage applications without worrying about the underlying infrastructure. It provides a simplified way to handle applications using a console, CLI, or APIs.

AWS Systems Manager: A unified interface that enables you to manage your AWS resources. It includes features like Run Command, Automation, Parameter Store, and more, making it easier to manage infrastructure at scale.
### What is AWS Elastic Beanstalk used for?
Elastic Beanstalk is a service for deploying and scaling web applications and services.
### How does AWS CloudFormation help in managing AWS resources?
I can use CloudFormation to modify and update the resources in your existing stacks in a controlled and predictable way
### What are the main components of AWS Global Infrastructure?
The  main components of the AWS Global Cloud Infrastructure are Regions, Availability Zones, Edge Locations, Wavelength Zones, and Regional Edge Caches.
### Which AWS services automatically run across multiple Availability Zones?
Several AWS services automatically operate across multiple Availability Zones (AZs) within a region to ensure reliability and fault tolerance. These include:

Amazon S3 (Simple Storage Service), which stores data redundantly across AZs for durability.
Amazon RDS (Relational Database Service) with Multi-AZ Deployment, providing automatic data replication and failover.
Amazon Aurora, which replicates data across AZs and supports automatic failover.
Amazon DynamoDB, offering multi-AZ data replication for high availability.
Amazon Elastic Load Balancing (ELB), distributing traffic across multiple AZs for reliability.
Amazon ECS (Elastic Container Service) with Fargate, balancing container tasks across AZs.
Amazon EFS (Elastic File System), automatically replicating data across AZs for availability.
Amazon Redshift, deploying clusters across AZs for automatic failover.
AWS Global Accelerator, improving application availability by directing traffic across AZs.
### What is the recommended best practice for deploying infrastructure in AWS?
The recommended method to deploy and manage infrastructure on AWS is to follow Infrastructure-As-Code (IaC) model using tools like AWS CloudFormation, AWS Cloud Development Kit (AWS CDK) or Terraform.




