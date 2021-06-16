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