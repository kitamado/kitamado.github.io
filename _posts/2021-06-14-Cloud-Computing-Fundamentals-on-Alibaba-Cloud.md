---
date: 2021-06-12
tags: coursera-quiz
title: Cloud Computing Fundamentals on Alibaba Cloud
status: ongoing
---
> https://www.coursera.org/specializations/alibabacloud

## Week1 ECS Quiz
1. What is the full name of ECS?
   - [x] Elastic Compute Service

2. Cloud disks are reliable because they use ________  to provide block-level data storage for ECS instances, ensuring 99.9999999% data reliability.

    - [x] a distributed file management system with 3 redundant copies

3. Which of the following products can be used to make an ECS only accessible from a private IP address?

    - [x] VPN Gateway

4. Alibaba Cloud server ECS is provided to customer as a cloud service. Which is the support SLA of Alibaba Cloud Products?
    - [x] 7*24

5. If you are running an online ticket booking service with relatively fixed traffic, which kind of payment method is the most appropriate?
    - [x] subsricption

6. Comparing to traditional server room trusteeship, ECS provides better flexibility. Which of the following operation is NOT supported?
   - [x] Modify available zone.

7. It's very easy to provision a new ECS instance. During the instance creation, you need to specify the Region and Zone. Which of the following description about region & zone is NOT correct?
   - [x] ECS has different support policy for different regions.

8. You can ________ an ECS instance’s configuration. (Number of correct answers: 2)

    - [x] upgrade
    - [x] downgrade

9. The most important feature of Alibaba cloud server is elasticity. When trying to expand the disk, user can expand the disk size or add a new disk. Which of the following description is NOT correct about adding a new disk?
    
    - [x] The size of the newly added disk must be bigger than the existing disk.

10. Before important operations such as upgrading application software or migrating business data, it is suggested to create one or more ________. 

    - [x] snapshots

## Week2 RDS Quiz

1. When doing RDS backup, which type of backup is supported by automatic backup?

    - [x] Physical Backup

2. After creating an RDS read-only instance, you should use which of the following services to make its data consistent to the master instance?

    - [ ] You have to configure the DTS service
    - [ ] You have to configure the Message Service
    - [ ] You have to configure the ExpressConnect Service
    - [x] Nothing, this will be done automatically by RDS

3. Which of the following is not Alibaba Cloud CloudMonitor metrics for RDS?

    - [x] Billing

4. If you have an ECS instance and an RDS instance in the same region, what is the easiest way to connect the two?

    - [x] Use the RDS Intranet Address and connect via Intranet

5. Which of the followings is part of the cost of using Alibaba Cloud RDS?

    - [x] Instance Fee

6. Which of the following statements is true for RDS?

    - [x] Multiple databases can be created in one RDS instance.

7. In each Alibaba Cloud service region, there are different data centers with independent power supply and network. These data centers are also called () in Alibaba Cloud.

    - [x] Zone

8. Which of the followings is not the database type supported by RDS?

    - [ ] PostgreSQL
    - [ ] Microsoft SQL Server
    - [ ] MySQL
    - [x] Oracle Database

7. When using Alibaba Cloud RDS, you still need to take care of which of the following O&M tasks?

    - [ ] Virtualization
    - [ ] Server hardware
    - [ ] Networking infrastructure
    - [x] Business data

8.  RDS is a PaaS, what is the full term of PaaS in cloud computing?

    - [x] Platform as a service

## Week3 OSS Quiz
1. Alibaba Cloud Object Storage Service (OSS) is a massive, highly available, secured and cost effective storage service. OSS is superior than self-built storage in all these aspects. Which of the following advantage relates to the high availability of OSS?

    - [ ] Availability actually relies on the underlying hardware, which can break down easily. Once the hard disk malfunctions, it can also lead to permanent data loss.


    - [x] Data Reliability is not less than 99.99999999%. Data is backed up automatically with multiple redundant copies.


   - [ ] Data has to be backed up by customer manually, which is time-consuming and labor-intensive.


    - [ ] The following features are available: Multiple Authentication and Authorization mechanism, Whitelist, Anti-leech URL, and Master-Sub Account

2. Alibaba Cloud Object Storage Service (OSS) is a massive, highly available, secured and cost effective storage service. One of the special characteristics of OSS is its superior data reliability, because of its underlying backup technology and policies. Which of the following statement about OSS backup is correct?
 
    - [ ] OSS supports 3 internal data copies, so the data can be  manually recovered should there be any problem.


    - [ ] Customer has to safeguard their own data. OSS provides various backup interfaces to facilitate offsite backups.


    - [ ] OSS leverages RAID0+1 configuration of its underlying physical hard disks. There is no impact even if 2 hard disks were to fail simultaneously.


    - [x] OSS supports 3 internal data copies, no human intervention is required to recover the data when anything goes wrong.

3. Alibaba Cloud OSS is a cloud storage service that features massive capacity, outstanding security, low cost, and high reliability. Files managed by OSS can be easily shared with external applications. Before sharing a file, you can find the URL of the file from the detail page of a file. The sharing is done by using ( ) application-layer protocol.

   - [ ] FTP


    - [x] HTTP


    - [ ] TCP


    - [ ] SMTP

4. After activating the OSS service, you must create buckets in the OSS management console or by using Open API before you can store files. Which of the following statements is true for buckets?

    - [x] Bucket names must be globally unique and cannot be changed once created.


    - [ ] Bucket names must be globally unique but can be changed after being created.


    - [ ] Bucket names must be unique under each account and can be changed after being created.


    - [ ] Bucket names must be unique under each account and cannot be changed once created.

5. OSS supports massive file storage and provides multiple file deletion functions.
 
    Which of the followings is most suitable if many objects need to be deleted with a pattern, for example, to delete all the objects generated before a specific day?

   - [ ] Deletes the objects one by one in the management console.


    - [ ] Deletes the objects in batch in the management console.

    - [x] Deletes the objects with lifecycle management.

    - [ ] Deletes the objects one by one using Open API.

6. In OSS, all data is stored in buckets. When an OSS bucket is set with the ( ) permission, the OSS Bucket allows other users to read (GET Object) the objects in the bucket.

    - [x] Public-read-write


    - [ ] Public-read


    - [ ] Private


    - [ ] Private-read

7. An object is the basic unit of data stored in OSS.  Which of the following file operations are supported by OSS? (Number of correct answers: 3)


    - [x] File modification


    - [ ] File uploading


    - [ ] File deletion


    - [ ] File reading

8. When using Alibaba Cloud OSS, you can set access control in 3 different levels, which are ( ) (Number of correct answers: 3)


    - [x] Bucket level


    - [x] Object level


    - [x] RAM account level


    - [ ] Directory level

9. In OSS Image Processing service, URLs are accessed with standard HTTP GET requests, and all processing parameters are in the QueyString of the URL. Which of the following modes are supported by image processing function?(Number of correct answers: 2)

    - [ ] Picture mode


    - [x] Parameter mode


    - [x] Style mode


    - [ ] Interactive mode

10. Which 2 parameters you need to configure to setup a static website hosted on an OSS bucket? (Number of correct answers: 2)

    - [x] Default page


    - [ ] Navigation page


    - [x] 404 page


    - [ ] Return page

## Week4 SLB Quiz
1. When using Alibaba Cloud SLB, users can enable the health check function. For Layer 4 services (UDP protocol), SLB determines the availability of ECS instances through?



    - [ ] Special characters contained in the message returned from backend ECS instances


    - [ ] Length of message returned from backend ECS instances 


    - [x] Whether it receives the required data packet from the backend ECS instance within the configured response timeout period or not.


    - [ ] Status codes returned from backend ECS instances 

2. Your website has high volume of traffic and sudden spikes for a very short time. In this scenario, which product can manage traffic peak efficiently and maintain a consistent user experience?



    - [ ] Auto Scaling


    - [x] Server Load Balancer
 


    - [ ] RDS


    - [ ] VPC

3. Applications or websites with users from different parts of the world will require low latency and high availability (HA) with multilayer disaster recovery.  In this scenario, except Auto Scaling should be used along with Server Load Balancer, which service is also suggested to be used together?



    - [ ] RDS


    - [ ] MaxCompute F


    - [x] DNS


    - [ ] VPC

4. Which feature in Server Load Balancer means that it can forward the access requests from a single user to the same ECS instance within a certain period to ensure session continuity?



    - [ ] Weighted Round Robin F


    - [x] Session persistence
 


    - [ ] Health check


    - [ ] Least connections scheduling

5. Server Load Balancer provides central certificate management system for which of the following protocol?



    - [ ] UDP


    - [ ] TCP


    - [ ] HTTP


    - [x] HTTPS

6. A company uses Alibaba Cloud SLB and Auto Scaling at the same time, hoping this combination can help save O&M cost and provide a stable and reliable system. 
 
    As an expert of Alibaba Cloud, which of the following statement is true?



    - [ ] All backend servers under the same SLB instance must be in the same Scaling Group  F


    - [ ] All ECS instances under the same SLB instance must be running on the same operating system


    - [ ] All backend servers under the same SLB instance must have the same configuration


    - [x] SLB instances must have Health Check enabled, or they cannot be used together with Auto Scaling

7. You are developing a highly available web application using stateless web servers. Which services are suitable for storing session state data?



    - [ ] OSS 


    - [x] Table Store


    - [x] RDS


    - [ ] MaxCompute

8. An enterprise built an isolated network environment by using Alibaba Cloud VPC, and connected this VPC and a traditional data center via VPN. As a result, this enterprise can seamlessly migrate data from its traditional data center to Alibaba Cloud.  Now they need to receive user requests from the Internet, and assign these requests to multiple ECS instances inside the VPC by using SLB. Which of the following statements are correct?

    - [x] They can create an SLB instance in the VPC, and mount ECS instances within the VPC to this SLB instance.  And then use a jump server to receive external requests, and direct these requests to SLB to forward them to backend ECS instances.


    - [ ] They can create an SLB instance in the VPC, and mount ECS instances within the VPC to this SLB instance. And then, bind an EIP to the SLB, so that this SLB instance can receive requests from the Internet, and assign these requests to the backend ECS instances.


    - [x] They can create an SLB instance with an Internet IP address, and mount ECS instances within the VPC to this SLB instance. The public SLB will be used to receive external requests. As a result, requests from the Internet will be transferred to backend ECS instances within the VPC.


    - [ ] They can create an SLB instance with an Internet IP address, and mount ECS instances within the VPC and servers of the traditional data center to this SLB instance. The public SLB will be used to receive external requests. As a result, requests from the Internet will be transferred to backend ECS instances within the VPC and servers of the traditional data center.

9. Usually, Alibaba Cloud SLB, ECS, and Auto Scaling are used together. Which of the following statements are correct? 



    - [x] SLB instances must have Health Check enabled, or they cannot be used in combination with Auto Scaling.


    - [x] An SLB instance can bind multiple Scaling Groups


    - [x] The three must be within the same region if they are going to be used in combination.


    - [ ] A Scaling Group can support multiple SLB instances simultaneously

10. Alibaba Cloud SLB is a service for distributing traffic among multiple ECS instances. To make SLB works as desired, you need to set which of the following configurations carefully. 



    - [x] SLB instance's property


    - [ ] SLB Instance's IP address


    - [x] SLB Instance's Listener


    - [x] SLB Instance's Backend ECS instance pool