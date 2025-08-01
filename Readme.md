
## 1) Understand Infrastructure as Code (IaC) concepts
#What is Terrafrom?
Terraform is an infrastructure as code tool that lets you build, change, and version cloud and on-prem resources safely and efficiently.

HOW DOES TERRAFORM WORK??

TERRAFORM >> TERRAFORM PROVIDER >>TARGET API
>Terraform creates and manages resources on cloud platforms and other services through their application programming interfaces (APIs)
TERRAFROM PROVIDERS:>>  AWS, AZURE,GCP,KUBERNETES,ALIBABA CLOUD,ORACLE CLOUD INFRASTRUCTURE.
Terraform create infra through APIs

Terraform work flow consist of three workflows
1)Write
>you might create a configuration to deploy an application on virtual machines in a Virtual Private Cloud (VPC) network with security groups and a load balancer.

2)Plan
>Terraform creates an execution plan describing the infrastructure it will create, update, or destroy based on the existing infrastructure and your configuration.

3)Apply

>On approval, Terraform performs the proposed operations in the correct order, respecting any resource dependencies. 

Eg:
     if you update the properties of a VPC and change the number of virtual machines in that VPC, Terraform will recreate the VPC before scaling the virtual machines.

Why Terraform?
HashiCorp co-founder and CTO Armon Dadgar explains how Terraform solves infrastructure challenges.

1)Manage any infrastructure
2)Track your infrastructure
3)Automate changes
4)Standardize configurations (MODULES)
5)Collaborate


#) Infrastructure as Code in a Private or Public Cloud

IaC and the Infrastructure Lifecycle?
>>IaC can be applied throughout the lifecycle, both on the initial build, as well as throughout the life of the infrastructure.
Commonly, these are referred to as Day 0 and Day 1 activities.

Day 0” code provisions and configures your initial infrastructure.

If your infrastructure never changes after the initial build (no OS updates, no patches, no app configurations, etc.) 

then you may not need tools that support subsequent updates, changes, and expansions.

Day 1” refers to OS and application configurations you apply after you’ve initially built your infrastructure.

If it is necessary to apply Day 1 through Day N configurations, the code might leverage a tool like Chef, Ansible, Docker, etc.

#) IaC Makes Infrastructure More Reliable
 >IaC makes changes idempotent, consistent, repeatable, and predictable.

#) IaC Makes Infrastructure More Manageable
>>During execution, Terraform will examine the state of the currently running infrastructure, determine what differences exist between the current state and the revised desired state, and indicate the necessary changes that must be applied. When approved to proceed, only the necessary changes will be applied, leaving existing, valid infrastructure untouched.


#)IaC Makes Sense



## To deploy infrastructure with Terraform:

Scope - Identify the infrastructure for your project.
Author - Write the configuration for your infrastructure.
Initialize - Install the plugins Terraform needs to manage the infrastructure.
Plan - Preview the changes Terraform will make to match your configuration.
Apply - Make the planned changes.


