# AWS SERVICE IMPLEMENTATION REPORT

Date: 09/03/2023
Company: Abstergo Industries
Responsible: Arthur de Assis Ferrande

## Introduction
This report presents the tool implementation process at Abstergo Industries, carried out by Arthur de Assis Ferrande. The objective of the project was to list 3 AWS services, in order to reduce immediate costs.

## Project description
The tool implementation project was divided into 3 stages, each with its specific objectives. The project stages are described below:

Step 1:
- Amazon EC2 (Elastic Compute Cloud)
- Provision instances for computational use, migrating "on premises" to the cloud.
- By using EC2, we can have greater flexibility, scalability and elasticity of use. By having your payment as "pay as you go" in the On Demand plan, we are able to cut costs right from the start, as we only pay for the computational capacity used, and the more we use it, the less we pay. You can further lower the cost by using the 1- to 3-year contract plans offered by AWS, such as Savings Plans or Reserved Instances. We can also link an Auto Scaling Group, together with a Load Balancer, making life easier for customers and system availability. We'll go into more detail about ASG in the next step. It is also important to provision in multi AZ, thus having protection against failures or interruptions.

Step 2:
- Auto Scaling
- As the name says, it automatically scales resources.
- Auto Scaling or Auto Scaling Group, in general, helps with the scalability/elasticity of certain items provisioned on AWS. As is the case with EC2 instances, among other features. With this, and the proper configuration, we no longer have idle resources, which when not necessary will be interrupted, keeping only the minimum amount that we decided or enough for the maintenance of the functionalities given the load of use required at a certain moment, consequently cutting expenses . The same is not possible on premise, unless we unplug part of our data center, which is generally not possible or recommended.
In case the demand is high, we avoid that our resources "bottleneck", because new resources will be automatically provisioned, and we can also decide a maximum amount to be provisioned. This helps both the overall availability of our system under a higher than normal load, and cost-cutting due to elasticity when that load is lower. Whereas, given the same situation on premise, when we needed to scale it, we would have a fixed cost beforehand, in addition to the time it would take for transport and assembly, without the option of reducing it when it was not being used, in addition to maintenance costs, energy, and the like.

Step 3:
- Database and Storage
- Use, management and storage of data, with greater efficiency and security.
- When migrating our database and storage to AWS, we have a few options, the main ones being: Amazon RDS or Aurora for relational databases, the second with MySQL and PostgreSQL compatibility, and the first with more options, but not only in what differ. And DynamoDB, among others for NoSQL. The advantages of migrating the database to the Cloud are the reduction of costs, in addition to the benefits of speed, monitoring, automatic recovery and self-scalability. In the case of Aurora, for example, the cost can be one tenth of the value of a commercial database. In RDS, on the other hand, savings of 40% can be achieved on average over a period of three years. Remembering that you only pay for what you use, in addition to the fees per instance executed. There is no need to worry about maintenance and storage, as you do not have to provision surplus in advance for future use.
When it comes to storage, we can carry it out in both Elastic Block Store and S3, depending on the case and need for use. Paying only for what we provision, in GB. With snapshots or versioning for backup, very high durability and availability. Again, the cost reduction comes from the lack of maintenance and hardware costs.

## Conclusion
The implementation of tools in the company Abstergo Industries aims to reduce expenses after migrating resources from on premise to the cloud, increasing the company's efficiency and productivity, and changing fixed expenses, and in advance - sometimes unnecessary - for flexible billing, along with scalability + business elasticity. It is recommended to continue using the implemented tools and search for new technologies that can further improve the company's processes.

## Attachments

https://aws.amazon.com/pt/ec2/  
https://aws.amazon.com/pt/ec2/pricing/  
https://docs.aws.amazon.com/pt_br/autoscaling/ec2/userguide/auto-scaling-groups.html  
https://docs.aws.amazon.com/pt_br/autoscaling/application/userguide/what-is-application-auto-scaling.html  
https://blog.awsfundamentals.com/unlocking-the-benefits-of-aws-rds-scaling  
https://docs.aws.amazon.com/pt_br/AmazonRDS/latest/AuroraUserGuide/Aurora.Integrating.AutoScaling.html#Aurora.Integrating.AutoScaling.Add  
https://aws.amazon.com/pt/rds/  
https://aws.amazon.com/pt/rds/pricing/  
https://aws.amazon.com/pt/rds/aurora/  
https://aws.amazon.com/pt/rds/aurora/pricing/  
https://aws.amazon.com/pt/rds/aurora/features/#High_Performance_and_Scalability  
https://aws.amazon.com/pt/ebs/  
https://aws.amazon.com/pt/ebs/pricing/  
https://aws.amazon.com/pt/s3/  
https://aws.amazon.com/pt/s3/pricing/?nc=sn&loc=4  

Signature of the Person Responsible for the Project:

Arthur de Assis Ferrande
