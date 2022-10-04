# AWS Cloud Security Principles and Frameworks 

## Separation of duties

In a cloud environment, there exists a line between the consumer role and the provider role, as there are things that AWS will do and things that the consumer will do. The perimeter of these responsibilities varies depending on the services used. 

## The different abstraction levels

The line is oblique because it needs to intercept different compute abstraction levels, such as hypervisors, containers, ands functions. The higher you go in the abstraction levels, the more the cloud provider can add value and can offload the consumer from non-strategic activities.

## The instance (or virtual machine) abstraction

Amazon Elastic Compute Cloud (Amazon EC2) is the service that allows AWS customers to launch instances in the cloud. When customers intercept us at this level, they retain responsibility of the guest operating system and above (middleware, applications, etc.) and their lifecycle. AWS has the responsibility for managing the hardware and the hypervisor including their lifecycle.

Amazon Lightsail is an easy way for customers to launch virtual private servers. Lightsail provides the resources for developers to deploy and manage websites and web applications in the cloud.

## The container abstraction

A container is a self-contained environment with soft boundaries that includes both your own application as well as the software dependencies to run it.

Modern containers-based solutions are usually implemented in two main logical pieces:

A containers control (orchestral) plane that is responsible for exposing the API and interfaces to define, deploy, and lifecycle containers.

A containers data plane that is responsible for providing capacity (as in CPU/Memory/Network/Storage) so that those containers can actually run and connect to a network. 

## The function abstraction

AWS Lambda is an event-driven, execution environment that allows an AWS customer to run a single function. So instead of having to manage and run a OS or container for the code, Lambda allows you to upload your code and let AWS figure out how to run it at scale. 

## The bare metal abstraction

AWS EC2 bare metal instances. In this case, customers are given direct access to hardware.

## The full container abstraction

AWS Fargate, a production-grade service that provides compute capacity to AWS containers control planes. This means the compute unit exposed to the user is the container abstraction, while AWS will manage transparently the data plane abstractions underneath.
