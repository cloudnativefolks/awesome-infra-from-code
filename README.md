 
Awesome Infrastructure from Code

## Introduction 
- The next evolution in infrastructure management is to derive your infrastructure directly from the application code, rather than defining it separately as code.
- Infrastructure-from-Code (IfC) analyzes your application code to automatically create and maintain the necessary cloud resources, eliminating the need for manual configuration. By inferring and exposing resources like web servers directly from the code, IfC abstracts infrastructure management, allowing companies to focus on their core services. While this new abstraction might seem daunting, it promises a significant productivity boost. Different IfC approaches share the common goal of letting service code define infrastructure needs, varying in how tightly they integrate with the code.

## Different approaches to Infrastructure from Code

- SDK-based solutions
- Code annotation-based solutions
- New programming languages
- Static code scanning

## IaC vs IfC

IaC really came into being throughout the 2010s. There are a lot of ways to use IaC, from Helm to Terraform to CloudFormation and beyond. And there are a lot of tools offering adjacent IaC solutions that have sprung up to help users, like Spacelift, Rancher, Pulumi and AWS CDK.


| Infrastructure as Code                                     | Infrastructure from Code                                    |
|------------------------------------------------------------|-------------------------------------------------------------|
| - Puts infrastructure needs and practices first.           | - Puts the infrastructure needs of the application first.    |
| - Creates an infrastructure source of truth that is ideally the VCS config, but can be a little hard to pin down if anyone strays from the config. | - Its source of truth is the app version, so VCS is built-in. |
| - Implements architecture & security best practices.       | - Scales to app needs, ensuring infrastructure is least privileged and rightsized. |
| - Can be difficult to manage and update over time.         | - Infrastructure for each app may follow the same standards, but will be unique to the app. |
| - Is often very one-size-fits-all.                         |                                                             |
