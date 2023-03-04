# Key review: Amazon EC2
<b>Amazon Elastic Compute Cloud (EC2)</b> is a web service provided by Amazon Web Services (AWS) that allows users to rent virtual servers, known as instances, on-demand in the cloud. EC2 provides a scalable and secure computing infrastructure, allowing users to launch and manage instances with a wide range of computing resources, including CPU, memory, storage, and network bandwidth.
Here are some key features of EC2:

## 1. Instance Types

EC2 offers a variety of instance types to meet different needs, including general-purpose, compute-optimized, memory-optimized, and storage-optimized instances. Each instance type has different CPU, memory, and storage configurations, providing customers with a broad range of options to choose from based on their specific use case.

Here are the main instance types available:

- <b>General Purpose</b>: General-purpose instances are designed for a balance of compute, memory, and networking resources. They are suitable for a wide range of workloads, such as web servers, small databases, and development/test environments. The current generation includes the T4g, M6g, M5, M5a, M5ad, M5d, and M4 instances.
- <b>Compute-Optimized</b>: Compute-optimized instances are designed for compute-intensive workloads that require high performance processors. They are ideal for running CPU-bound applications, such as batch processing, high-performance computing (HPC), and scientific modeling. The current generation includes the C6g, C5, C5a, C5ad, C5d, and C4 instances.
- <b>Memory-Optimized</b>: Memory-optimized instances are designed for memory-intensive workloads that require high memory resources. They are ideal for running large-scale in-memory databases, such as SAP HANA, Apache Spark, and Memcached. The current generation includes the R6g, R5, R5a, R5ad, R5d, and R4 instances.
- <b>Storage-Optimized</b>: Storage-optimized instances are designed for storage-intensive workloads that require high disk I/O performance. They are ideal for running data-intensive applications, such as big data analytics, NoSQL databases, and data warehousing. The current generation includes the D3, H1, and I3 instances.
- <b>Accelerated Computing</b>: Accelerated computing instances are designed for workloads that require GPU or FPGA acceleration. They are ideal for running machine learning, video encoding, and other GPU/FPGA-intensive applications. The current generation includes the G4, P3, P3dn, Inf1, and F1 instances.
- <b>Bare Metal</b>: Bare metal instances provide direct access to the underlying hardware and are ideal for running applications that require access to physical resources, such as high-performance databases and HPC clusters. The current generation includes the i3.metal, c5.metal, m5.metal, r5.metal, and z1d.metal instances.

Each instance type also has different pricing options, with on-demand, reserved, and spot instances available. Users can choose the instance type that best fits their workload and budget requirements, making EC2 a flexible and scalable computing solution.

## 2. Operating Systems

EC2 supports a wide range of operating systems, including popular Linux distributions such as Amazon Linux, Ubuntu, and Red Hat Enterprise Linux, as well as Microsoft Windows Server and other operating systems.

## 3. Security

EC2 provides several security features, including virtual private cloud (VPC), security groups, network access control lists (ACLs), and IAM roles. These features allow users to control who can access their instances and network resources, as well as provide encryption and authentication options.

Here are some of the key security features available in EC2:

- <b>Virtual Private Cloud (VPC)</b>: EC2 instances can be launched within a virtual private cloud (VPC), which allows users to define a private network topology within the AWS cloud. VPCs provide a secure and isolated environment for instances, allowing users to control inbound and outbound network traffic with network access control lists (ACLs) and security groups.
- <b>Security Groups</b>: EC2 security groups act as virtual firewalls for instances, controlling inbound and outbound traffic to instances. Security groups are stateful, which means that any traffic allowed in is also allowed out, and vice versa. Users can create and manage security groups to control access to instances.
- <b>Network Access Control Lists (ACLs)</b>: Network ACLs act as a firewall for subnets in a VPC, controlling traffic at the subnet level. Network ACLs allow users to create rules to allow or deny traffic to and from subnets.
- <b>Identity and Access Management (IAM) Roles</b>: IAM roles allow users to delegate permissions to EC2 instances, enabling them to access other AWS resources, such as S3 buckets or DynamoDB tables, without needing to manage credentials or keys.
- <b>Encrypted EBS Volumes</b>: EC2 instances can be configured to use encrypted Elastic Block Store (EBS) volumes, which provide additional data protection. Encrypted EBS volumes use industry-standard AES-256 encryption to encrypt data at rest, and the encryption keys are managed by AWS Key Management Service (KMS).
- <b>Secure Shell (SSH) Key Pairs</b>: EC2 instances can be accessed using SSH key pairs, which provide secure authentication for Linux instances. SSH key pairs allow users to securely access instances without needing to use a password.
- <b>AWS Shield</b>: AWS Shield is a managed DDoS protection service that helps protect EC2 instances from DDoS attacks. AWS Shield provides a standard service level for all AWS customers, and an advanced service level for customers who require additional protection.

Overall, Amazon EC2 provides a range of security features to help users protect their instances and data in the cloud. Users can configure security groups, network ACLs, IAM roles, encrypted EBS volumes, SSH key pairs, and AWS Shield to provide a comprehensive security solution for their EC2 instances.

## 4. Elastic Block Store (EBS)

<b>Amazon Elastic Block Store (EBS)</b> is a cloud-based block storage service that provides persistent storage for EC2 instances. EBS volumes are network-attached, which means they can be attached and detached from EC2 instances as needed, and they can be used to store data that requires long-term persistence, such as databases, file systems, and application data.

Here are some of the key features and benefits of EBS:

- <b>Performance</b>: EBS provides consistent and low-latency performance, with the ability to scale up or down as needed. EBS volumes support different volume types, including General Purpose (GP2), Provisioned IOPS (IO1), Throughput Optimized (ST1), and Cold HDD (SC1), which offer different levels of performance and cost.
- <b>Availability</b>: EBS volumes are designed for high availability, with data replicated within the same availability zone (AZ) to protect against hardware failures. Users can also create snapshots of EBS volumes, which can be stored in Amazon S3 for additional data protection and disaster recovery.
- <b>Durability</b>: EBS volumes are designed for durability, with data automatically replicated within the same AZ. In addition, users can create point-in-time snapshots of EBS volumes, which can be used to restore volumes in case of data loss or corruption.
- <b>Elasticity</b>: EBS volumes can be attached and detached from EC2 instances as needed, and they can be scaled up or down in size and performance to meet changing workload requirements. This makes EBS a flexible and scalable storage solution for EC2 instances.
- <b>Encryption</b>: EBS volumes can be encrypted using AWS Key Management Service (KMS), which provides additional security for data at rest. Encrypted EBS volumes use industry-standard AES-256 encryption, and the encryption keys are managed by AWS KMS.
- <b>Integration with other AWS Services</b>: EBS integrates with other AWS services, such as Amazon RDS, Amazon Redshift, and Amazon EMR, to provide storage for these services. EBS volumes can also be used with AWS Elastic Beanstalk and AWS CloudFormation to automate the deployment of EC2 instances and applications.

Overall, EBS provides a reliable, durable, and scalable block storage solution for EC2 instances, with the ability to choose different volume types and encryption options to meet specific storage requirements. EBS volumes can be easily attached and detached from instances, and they integrate with other AWS services to provide a seamless storage solution for cloud-based applications.

## 5. Auto Scaling

<b>Auto Scaling</b> is a service provided by Amazon Web Services (AWS) that allows users to automatically scale resources, such as EC2 instances, based on the changing demands of their applications or workloads. With Auto Scaling, users can ensure that their applications are running optimally at all times, without having to manually manage the scaling process.

Here are some key features and benefits of Auto Scaling:

- <b>Scalability</b>: Auto Scaling allows users to automatically add or remove EC2 instances based on the changing demands of their applications or workloads. This ensures that applications are able to handle sudden spikes in traffic, without having to worry about provisioning additional resources manually.
- <b>Cost Savings</b>: Auto Scaling helps users save costs by automatically scaling resources up or down based on actual usage. This helps ensure that users only pay for the resources they need, and not for unused or underutilized resources.
- <b>Availability</b>: Auto Scaling helps improve application availability by automatically scaling resources in response to changes in demand. This helps ensure that applications are always available, even during peak periods of usage.
- <b>Elasticity</b>: Auto Scaling allows users to scale resources elastically, based on the actual demand for their applications or workloads. This means that users can quickly and easily add or remove resources as needed, without having to worry about manual provisioning or deprovisioning.
- <b>Flexibility</b>: Auto Scaling is highly configurable, allowing users to define scaling policies that are tailored to the specific needs of their applications or workloads. This means that users can control how and when resources are added or removed, based on a variety of metrics and criteria.
- <b>Integration</b>: Auto Scaling integrates with other AWS services, such as Elastic Load Balancing and CloudWatch, to provide a complete solution for managing application workloads. Users can use Auto Scaling in conjunction with these services to ensure that their applications are always available and performing optimally.

Overall, Auto Scaling is a powerful tool for managing resources in the cloud, allowing users to automatically scale resources up or down based on the changing demands of their applications or workloads. With its scalability, cost savings, availability, elasticity, flexibility, and integration features, Auto Scaling is a key component of a robust and resilient cloud infrastructure.
## 6. Monitoring and Management

Monitoring and management are important aspects of running EC2 instances in the AWS cloud. AWS provides a number of tools and services to help users monitor and manage their EC2 instances, including Amazon CloudWatch and AWS Systems Manager.

<b>Amazon CloudWatch</b> is a monitoring service that provides users with real-time and historical metrics for their EC2 instances, as well as other AWS resources. CloudWatch can be used to monitor CPU usage, network traffic, disk I/O, and other metrics, and it can send alerts when thresholds are breached. CloudWatch can also be used to monitor custom metrics that users define themselves.

<b>AWS Systems Manager</b> is a management service that provides users with a suite of tools to manage and automate their EC2 instances. Systems Manager can be used to configure instances, apply software updates, and patch instances for security vulnerabilities. It can also be used to automate common administrative tasks, such as running scripts and executing commands across multiple instances at once.

Here are some key features and benefits of monitoring and management in EC2:

- <b>Real-time monitoring</b>: Amazon CloudWatch provides real-time monitoring of EC2 instances and other AWS resources, giving users insight into the health and performance of their applications.
- <b>Historical data</b>: CloudWatch provides historical data on metrics, allowing users to analyze trends and identify performance issues over time.
- <b>Alarms and alerts</b>: CloudWatch can be used to set alarms and send alerts when metrics exceed specified thresholds, enabling users to proactively address issues before they become problems.
- <b>Automated management</b>: AWS Systems Manager provides tools for automated management of EC2 instances, allowing users to configure, patch, and automate common administrative tasks across multiple instances at once.
- <b>Cost savings</b>: By using monitoring and management tools like CloudWatch and Systems Manager, users can identify and address issues that can result in higher costs, such as underutilized instances or inefficient resource usage.
- <b>Integration</b>: CloudWatch and Systems Manager integrate with other AWS services, such as AWS Lambda and AWS Config, to provide a comprehensive suite of monitoring and management tools for EC2 instances and other AWS resources.

Overall, monitoring and management are critical components of running EC2 instances in the AWS cloud. By leveraging tools like CloudWatch and Systems Manager, users can gain insight into the performance and health of their instances, automate common administrative tasks, and identify and address issues before they become problems. This helps ensure that applications running on EC2 instances are always available and performing optimally.