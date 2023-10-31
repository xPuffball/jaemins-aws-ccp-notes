## A Traditional IT Overview
### How Websites Work
---
We want to use a network between ourselves (client) and a server. We will find a network and use it to route packets through it to the server, which will also reply.

For clients to find the server and vice versa, both clients and servers must have **IP Addresses**.

### What is a Server Composed Of?
---
- **Compute:** CPU
- **Memory:** RAM
- **Storage:** Data
	- Database: Store data in a structured way
- **Network:** Routers, switch, DNS server

### IT Terminology
---
>**Definition: Network**
>Cables, routers, and servers connected with each other

>**Definition: Router**
>A networking device that forwards data packets between computer networks. They know where to send your packets on the internet!

>**Definition: Switch**
>Takes a packet and sends it to the correct/client on your network.

### Problems with Traditional IT Approach
---
- Need physical space for data center
- Costs for power supply, cooling, maintenance
- Adding and replacing hardware takes time
- Scaling is limited
- Hire 24/7 team to monitor the infrastructure
- How to deal with disasters? (earthquake, power shutdown, fire)
Is there a way to externalize all this...?

**Yes!** (see below)

## What is Cloud Computing?
---
>**Definition: Cloud Computing**
>The **on-demand delivery** of compute power, database storage, applications and other IT resources.

**Features of Cloud Computing:**
- **Pay-as-you-go** pricing **(flexible pricing)**
- You can **provision exactly the right type and size of computing resources** you need **(flexible scaling)**
- You can access as many resources as you need, **almost instantly** **(speed)**
- Simple way to access **servers, storage, databases**, and a set of application services **(abstraction)**

So we are just using Amazon's data centers/hardware with a nice web interface.
(Gmail, Dropbox, Netflix is cloud computing!)

### The Deployment Models of the Cloud
---
>**Definition: Private Cloud**
>Cloud services used by a single organization, not exposed to the public.

Use **Private Cloud** if you need:
- Complete control
- Security for sensitive applications
- Meet specific business needs
#### Public Cloud
>**Definition: Public Cloud**
>Cloud resources owned and operated by a third-party cloud service provider delivered over the Internet

(Advantages are listed above!)
(The Big 3: AWS, Azure, GCP)
#### Hybrid Cloud
>**Definition: Hybrid Cloud**
>Keeping some servers on premises and extending some capabilities to the Cloud

Use **Hybrid Cloud** if you need:
- Control over the sensitive assets in your private infrastructure
- Exposure to flexibility and cost-effectiveness of public cloud

### The Five Characteristics of Cloud Computing
---
#### 1. On-demand self service
- Users can provision resources and use them without human interaction from the service provider
#### 2. Broad network access
- Resources available over the network, and can be accessed by diverse client platforms
#### 3. Multi-tenancy and resource pooling
- Multiple customers can share the same infrastructure and applications with security and privacy
- Multiple customers are serviced from the same physical resources
#### 4. Rapid Elasticity and Scalability
- Automatically and quickly acquire/dispose resources when required
#### 5. Measured service:
- Usage is measured, and users pay exactly for what they have used

### The Six Advantages of Cloud Computing
---
#### 1. Trade Capital Expenses (CAPEX) for operational expense (OPEX)
- Pay On-Demand: Don't own hardware
- Reduced Total Cost of Ownership (TCO) & Operational Expense (OPEX)
#### 2. Benefit from Massive Economies of Scale
- Prices are reduced as AWS is more efficient due to large scale
#### 3. Stop Guessing Capacity
- Scale based on actually measured usage
#### 4. Increase Speed and Agility

#### 5. Stop spending money running and maintaining data centres

#### 6. Go global in minutes
- Leveraging the AWS global infrastructure

### The Six Problems Solved by the Cloud
---
#### 1. Flexibility
- Change resource types when needed
#### 2. Cost-Effectiveness
- Pay as you go, for what you use
#### 3. Scalability
- Accommodate larger loads by making hardware stronger or adding additional nodes
#### 4. Elasticity
- Ability to scale out and scale-in when needed
#### 5. High-availability and fault-tolerance
- Build across data centres
#### 6. Agility
- Rapidly develop, test, and launch software applications

## The Different Types of Cloud Computing
### Types of Cloud Computing
---
#### Infrastructure as a Service (IaaS)
- Provide building blocks for cloud IT
- Provides networking, computers, data storage space
- Highest level of flexibility
- Easy parallel with traditional on-premises IT
#### Platform as a Service (PaaS)
- Removes the need for your organization to manage the underlying infrastructure
- Focus on the deployment and management of your applications
#### Software as a Service (SaaS)
- Completed product that is run and managed by the service provider
#### **Examples of Cloud Computing Types**

![[Pasted image 20231030223641.png|400]]

**Infrastructure as a Service**
- Amazon EC2 (on AWS)
- GCP, Azure, Rackspace, Digital Ocean, Linode
**Platform as a Service**
- Elastic Beanstalk (on AWS)
- Heroku, Google App Engine (GCP), Windows Azure (Microsoft)
**Software as a Service**
- Many AWS services (ex: Rekognition for Machine Learning)
- Google Apps (Gmail), Dropbox, Zoom

### Pricing of the Cloud - Quick Overview
---
AWS has 3 pricing fundamentals, following the pay-as-you-go pricing model
#### Compute:
- Pay for compute time
#### Storage:
- Pay for data stored in the cloud
#### Data transfer OUT of the Cloud:
- Data transfer IN is free!

(and this solves the expensive issue of traditional IT!)

## AWS Cloud Overview

### AWS Cloud Use Cases
---
- AWS enables you to build sophisticated, scalable applications
- Applicable to a diverse set of industries
- Use cases include
	- Enterprise IT, Backup & Storage, Big Data analytics
	- Website hosting, Mobile & Social Apps
	- Gaming

### AWS Global Infrastructure
---
#### AWS Regions
AWS has **Regions** all around the world...
- Names can be us-east-1, eu-west-3...

>**Definition: Region**
>A cluster of data centers, and most AWS services are region-scoped.

### How do you choose an AWS Region?
---
The factors to consider when launching a new AWS application:
#### Compliance
- With data governance and legal requirements: Data never leaves a region without your explicidt permission.
#### Proximity
- To customers: this means reduced latency!
#### Available Services
- Within a Region: new services and new features aren't available in every region, so watch out!
#### Pricing
- Pricing varies region to region and is transparent in the service pricing page!

### AWS Availability Zones
---
Each region has many availability zones (usually 3, min is 3, max is 6)
**Example:**
- ap-southeast-2a
- ap-southeast-2b
- ap-southeast-2c 
Each availability zone (AZ) is one or more discrete data centers with redundant power, networking, and connectivity. They're separate from each other, so that they're isolated from disasters!

- Also connected w/ high bandwidth, ultra-low latency networking

### AWS Points of Presence (Edge Locations)
---
