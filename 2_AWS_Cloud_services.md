# AWS Virtual Private Cloud (VPC)

- Creates a private network inside AWS, that is similar to creating on premises network. 
- Complete control on 
  - **IP address spaces**: A unique string of numbers seperated by `.` that is used to identify each computer that communicates using 
    Internet Protocols to communicate over networks. 
  - **Subnets**: It is a logical partition of the network into multiple smaller networks to increase efficiency. 
  - **Routing Tables**: It is the set of rules often viewed in table format, that is used to determine where data packets will be directed. 
  - **Network ACL**: It is an additional layer that is used to enhance security, to control data in and out of subnet. (ACL = Access Control List)
  
- To further enhance security we can:
  - To isolate subnets 
  - Defining ACLs
  - Customising rules of routing table 

- AWS Account -> VPC IP Address space -> Divided into several subnets 
  -> Some subnets can be connected to the Internet Gateway through routing table 
  
# Security Groups in AWS 

- These are built in firewalls in the Amazon VPC. 
- Go to security groups menu and for any compute instance we can add security groups to them. 

# Amazon Compute Services
- **EC2**: They are virtual server instance type that can host web services to large ML clusters.
  - We can change the instance type as well.  
- **Lambda**: It helps you run code without managing servers.
  - Pay only for execution hours 
- **LightSail**: Runs simple websites and lauch a virtual private server. 
- **ECS**: Container manager used to manage Docker containers and clusters. 

# Amazon Elastic Compute Cloud (EC2)
- AMI (Amazon Machine Images) are the basic building blocks of EC2. 
- It is a template that contains the software configurations like OS, applications, servers etc. 
- They are used to launch an instance  

# Amazon Lambda
- It helps you run code without managing servers.
- When to choose?
  - When we don't want to maintain OS and other server stuff
  - When we need standalone code execution and then use or store the results somewhere. 

# Amazon Elastic Beanstalk 
- It is a PAAS, it is used to deploy, create and test. 
- It is ready to use for deploying and scaling. 
- The following are the components of Elastic Beanstalk:
  - Operating System 
  - HTTP Service 
  - Application Service
  - Language interpreter
  - Host
- Lambda vs Beanstalk
  - Lambda is cheaper 
  - Lambda is function as a service, Beanstalk is platform as a service 
  - Lambda runs scripts, Beanstalk run app  

# Application Load Balancer 
- Distributes incoming network or application traffic. 

# Amazon Storage Services 
- **S3**: It is an object storing facility. It has a very high durabilty. Benefits:
  - Stores data in bucket- each bucket upto 5TB
  - Data download 
  - Standard Interfaces 
  - Permissions 
  
- **S3 Galcier**: It is secure, durable and extremely low cost storage for data archive and long-term backup
  - Query in place functionality, for better insights
  - Data Retrival time: 
   -  Expedited: 1-5 min
   -  Standard: 3-5 hours
   -  Bulk: 5-12 hours
   
-  **S3 vs Glacier:**
  - Avg Latency : ms | min/hours
  - Cost : $$ | $

- **Elastic Book Store**: Provides block level storage for EC2 instances. They exist seperately from the life cycle of the instance.
  - They act like raw, unformatted hard drive. 


# Amazon Database Services 

- **Amazon RDS**: Relational database. 
  - They can be scalled independently
  - Doesnot give shell access to DB instance. 
  
- **Dynamo DB**:  It is a no SQL database
  - Provides encryption at rest  

- **Redshift**: It is a peta-byte scale data warehouse. 
  - They offer fast query service despite of large data
  - First we need to set up nodes known as Amazon Redshift cluster.

- **Aurora**: Fully managed RDS
  - 5x faster than mySQL
  - 3x faster than Postgres
  
 
