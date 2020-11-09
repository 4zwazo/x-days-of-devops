# Cloud Fundamentals

### Day 1 - Cloud Computing

#### November 7, 2020

**Focus**: The focus was on understanding what cloud computing is all about.

**Progress**:

- Creating free-tier account
- Leran the basics of cloud computing
- Learn about cloud deployment models
- Learn about the benefits of these models
- Learn about the shared responsibility model

**Thoughts**:\ Not much hands-on practice today. But learning about cloud computing is refreshing.

**Work & Resources**:\
[Shared Responsibility Model](https://aws.amazon.com/compliance/shared-responsibility-model/)

<hr>

### Day 2 - Foundational & Compute Service

#### November 8, 2020

**Focus**: The focus for today was on Virtual Private Cloud (VPC).

**Progress**:

- Learn the importance of the VPC
- Lean about subnets, route tables, security groups, internet gateway, etc
- Understanding the default VPC
- Understanding Region and Availability Zone, and their impact
- Creating custom VPC
- Launch EC2 instances and connect to then via ssh

**Thoughts**: Creating a custom VPC was challenging. With persistence and perseverance I was able to get it done. I am longer using the default VPC.

**Work & Resources**:\
[Virtual private cloud](https://en.wikipedia.org/wiki/Virtual_private_cloud)\
[Amazon VPC Documentation](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)\

![Custom VPC](images/custom-vpc.jpg)

<hr>

### Day 3 - Foundational & Compute Service

#### November 9, 2020

**Focus**: No better way to start with AWS than EC2. Today the learning focuses on EC2 basics and some of the main features it offers. It also touches on storage, auto scaling and load balancing.

**Progress**:

EC2-Basics:

- Learned how to create EC2 instance
- Associate the instance with a security group that allows ssh traffic from any IP
- Create a snapshot of the EBS volume attached to the EC2 Instance
- Create an AMI using the snapshot
- Create a new instance using the AMI

Storage:

- Learn about the different storage class
- Create an EBS volume and attack it to instance
- Create an EFS filesystem and mount it to instance

S3 and IAM Role:

- Create an S3 bucket
- Create IAM Role with EC2 Service
- Attach AmazonS3FullAccess to policy
- Attach role when creating launch configuration

Auto scaling and Load Balancing

- Create launch configuration (useing ami-03657b56516ab7912)
- Create autoscaling group using the launch configuration
- Create target groups
- Create load balancer and have load balancer serves traffic to the instance
- Verify you can see webapp from your browser

**Thoughts**: Doing the lab was refreshing and really cement the concept for me. Navigating the console was a bit intimidating at first. With patience and dedication it becomes easier. Taking the time to draw the architecture prior immersing in the labs was instrumental in connecting the dots.

**Work & Resources**:

![EC2](images/day-1-1.png)
