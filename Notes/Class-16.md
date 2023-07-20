# AWS: Cloud Servers

## AWS EC2

**What is an EC2 Instance?**

- Amazon Elastic Compute Cloud (Amazon EC2) offers the broadest and deepest compute platform, with over 600 instances and choice of the latest processor, storage, networking, operating system, and purchase model to help you best match the needs of your workload.

**Name 2 use cases for EC2.**

- Migrate and build apps with ease using AWS Migration Tools, AWS Managed Services or Amazon Lightsail

**Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.**

- One reason to use Amazon Elastic Container Service (ECS) instead of services like Heroku, Digital Ocean, or Render.com is the flexibility and control it offers over your containerized applications. With ECS, you have fine-grained control over the deployment, configuration, and scaling of your containers. You can use the AWS Management Console or the AWS Command Line Interface (CLI) to define the resources, networking, and security settings for your containers. This level of control allows you to tailor your application environment to specific requirements, such as performance optimizations or security configurations. Additionally, ECS integrates seamlessly with other AWS services, such as Amazon EC2, Elastic Load Balancing, Amazon RDS, and Amazon CloudWatch. This integration enables you to build a highly scalable and resilient application stack, taking advantage of the rich set of AWS services and features. While services like Heroku, Digital Ocean, or Render.com provide simplified deployment options, they may have limitations in terms of customization or integration with other services. If you have specific requirements or want full control over your containerized applications, ECS offers a robust and flexible solution within the AWS ecosystem.

## EC2 For Humans

**Where can we find EC2 on the AWS Console?**

- You can find EC2 on the AWS Console by searching for "EC2" in the search bar at the top of the page and clicking on "Amazon EC2" in the search results.


**Explain the general difference between T2 Micro and XL.**

- T2 Micro is a smaller instance type with lower resources, suitable for lightweight applications. T2 XL is a larger instance type with more resources, capable of handling more demanding workloads.

**Explain a “Compute Cycle” to a non-technical friend.**

- A compute cycle is like a single step or action taken by a computer to solve a problem or complete a task. Computers perform many compute cycles to process data and perform tasks efficiently.

## Elastic Beanstalk

**What is Elastic Beanstalk?**

- Elastic Beanstalk is a fully managed service provided by AWS that simplifies the deployment and management of applications. It allows developers to quickly deploy their applications onto AWS infrastructure without worrying about the underlying infrastructure setup.

**Describe the relationship between EC2 and Elastic Beanstalk.**

- Elastic Beanstalk utilizes EC2 instances as the underlying infrastructure to deploy and run applications. It automatically provisions and manages the EC2 instances, load balancers, and other necessary resources required to host the application, abstracting away the complexity of directly managing EC2 instances.

**Name some benefits of using Elastic Beanstalk.**

- Easy application deployment: Elastic Beanstalk streamlines the deployment process, handling infrastructure provisioning and resource management automatically, allowing developers to focus more on writing code.

- Scalability: Elastic Beanstalk provides built-in scaling capabilities, allowing applications to automatically scale up or down based on demand, ensuring optimal performance.

- Monitoring and management: Elastic Beanstalk integrates with AWS services like CloudWatch, providing monitoring and logging capabilities to track application performance and diagnose issues.

- Environment management: Elastic Beanstalk enables the creation of multiple environments (such as development, testing, production) for an application, making it easier to manage different stages of the application lifecycle.

- Multiple language and platform support: Elastic Beanstalk supports a variety of programming languages and platforms, providing flexibility and compatibility for different types of applications.