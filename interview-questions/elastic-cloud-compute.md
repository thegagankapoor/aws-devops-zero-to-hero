### 1. What is Amazon EC2?
Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides virtual machines in the cloud. It allows users to create, configure, and manage virtual servers (known as instances) in the AWS cloud, Instead of buying and maintaining physical servers, you rent virtual machines from AWS and pay only for what you use.

Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides resizable compute capacity in the cloud. It allows users to rent virtual servers on demand and scale your computing resources up or down based on your needs.

### 2. How does Amazon EC2 work?
Amazon EC2 enables users to launch instances based on pre-configured Amazon Machine Images (AMIs). These instances run within virtual private clouds (VPCs) and can be configured with various resources like CPU, memory, storage, and networking.

### 3. What are the different instance types in EC2?
Amazon EC2 offers a wide range of instance types optimized for different use cases, such as general-purpose, memory-optimized, compute-optimized, and GPU instances.

## 🔹 EC2 Instance Families

1. **General Purpose (T, M)**

   * Balanced CPU, memory, and networking.
   * Good for websites, dev/test, small apps.
   * Examples: `t2.micro`, `t3.medium`, `m5.large`.

2. **Compute Optimized (C)**

   * High CPU power.
   * Best for heavy computation, game servers, batch processing.
   * Examples: `c5.large`, `c6g.xlarge`.

3. **Memory Optimized (R, X, z)**

   * Large RAM compared to CPU.
   * Best for databases, caching, in-memory analytics.
   * Examples: `r5.large`, `x1e.xlarge`.

4. **Storage Optimized (I, D, H)**

   * High disk throughput & storage capacity.
   * Best for big data, data warehousing, Hadoop, Elasticsearch.
   * Examples: `i3.large`, `d2.xlarge`.

5. **Accelerated Computing (P, G, F, Inf, Trn)**

   * Use GPUs or FPGAs.
   * Best for machine learning, AI, 3D rendering, video processing.
   * Examples:

     * `p4d` (NVIDIA GPU for ML training).
     * `g5` (graphics).
     * `f1` (custom hardware on FPGA).

---

## 🔹 Super Easy Way to Remember 🌟

* **T/M → Typical (General)**
* **C → Compute-heavy**
* **R/X → RAM-heavy**
* **I/D/H → IO-heavy (storage)**
* **P/G/F → Powerful (GPUs/FPGAs for AI)**

---

👉 So the “formula” is:
**General → Compute → Memory → Storage → GPU/Accelerated**

### 4. Explain the differences between on-demand, reserved, and spot instances.
- On-Demand Instances: Pay-as-you-go pricing with no upfront commitment.
- Reserved Instances: Provides capacity reservation at a lower cost in exchange for a commitment.
- Spot Instances: Allows users to bid on unused EC2 capacity, potentially leading to significantly lower costs.

### 5. How can you improve the availability of EC2 instances?
To improve availability, you can place instances in multiple Availability Zones (AZs) within a region. This helps ensure redundancy and fault tolerance.

### 6. What is an Amazon Machine Image (AMI)?
An Amazon Machine Image (AMI) is a pre-configured template that contains the information required to launch an EC2 instance. AMIs can include an operating system, applications, data, and configuration settings.

### 7. How can you secure your EC2 instances?
You can enhance the security of EC2 instances by using security groups, Network ACLs, key pairs, and configuring firewalls. Additionally, implementing multi-factor authentication (MFA) is recommended for account access.

### 8. Explain the difference between public IP and Elastic IP in EC2.
A public IP is assigned to an instance at launch, but it can change if the instance is stopped and started. An Elastic IP is a static IP address that can be associated with an instance, providing a consistent public IP even after stopping and starting the instance.

### 9. How can you scale your application using EC2?
You can scale your application horizontally by adding more instances. Amazon EC2 Auto Scaling helps you automatically adjust the number of instances based on demand.

### 10. What is Amazon EBS?
Amazon Elastic Block Store (EBS) provides persistent block storage volumes for EC2 instances. EBS volumes can be attached to instances and used as data storage.

### 11. How can you encrypt data on EBS volumes?
You can encrypt EBS volumes using Amazon EBS encryption. You can choose to create encrypted volumes during instance launch or encrypt existing unencrypted volumes.

### 12. How can you back up your EC2 instances?
You can create snapshots of EBS volumes, which serve as backups. These snapshots can be used to create new EBS volumes or restore existing ones.

### 13. What is the difference between instance store and EBS-backed instances?
Instance store instances use ephemeral storage that is directly attached to the instance, providing high I/O performance. EBS-backed instances use EBS volumes for storage, offering persistent data storage.

### 14. What are instance metadata and user data in EC2?
Instance metadata provides information about an instance, such as its IP address, instance type, and IAM role. User data is information that you can pass to an instance during launch to customize its behavior.

### 15. How can you launch instances in a Virtual Private Cloud (VPC)?
When launching instances, you can choose a specific VPC and subnet. This ensures that the instances are launched within the defined network environment.

### 16. What is the purpose of an EC2 security group?
An EC2 security group acts as a virtual firewall for instances to control inbound and outbound traffic. You can specify rules to allow or deny traffic based on IP addresses and ports.

### 17. How can you automate the deployment of EC2 instances?
You can use AWS CloudFormation to create and manage a collection of related AWS resources, including EC2 instances. This allows you to define the infrastructure as code.

### 18. How can you achieve high availability for an application using EC2?
You can use features like Amazon EC2 Auto Scaling and Elastic Load Balancing to distribute incoming traffic and automatically adjust the number of instances to handle changes in demand.

### 19. What is Amazon Machine Learning (Amazon ML)?
Amazon ML is a service that enables you to build predictive models using machine learning technology. It's used to perform predictions on data and make informed decisions.

### 20. What is Amazon EC2 Instance Connect?
Amazon EC2 Instance Connect provides a simple and secure way to connect to your instances using Secure Shell (SSH). It eliminates the need to use key pairs and allows you to connect using your AWS Management Console credentials.
