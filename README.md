# learning-AWS

##### Cloud Computing characterstics
* On Demand
  * You get what need when required.
  * VM, Storage,Database etc
* Broad Network Access
  * Private network
  * public network
  * Access to the network
* Resource Polling
  * Network, Rack, Building are shared among mutiple clients/tenants.
* Rapid Elasticity
  * Scale in/out things on demand.
  * Eg add/reduce storage, database, VM.
* Measured Service
  * Pay as you go or Pay for what you use.


##### Service Models
* Infrastructure as a service.  
* Platform as a service.
* Software as a service.

##### Regions
* Place where paticular resource is located.
* More than **14** regions across the world.
* A region can be used based on enduser to reduce **latency**.
* A region can be used based on **cost effectiveness**. Cost vary accross regions.
* Security Compliance.
* Choose multiple regions.

##### Availability Zones
* Each **region** can have multiple zones.
* Collection of data centres connected with private fibres.
* Provide **High availability**.
* Fault **Tolerance**.
* Eg Oregon region (us-west-a, us-west-b,us-west-c)

###### Edge Location
* Amazon cloud front
  * deliver content quickly.
  * Cache content at edge location.
* Amazon route53
  * DNS query.
  * Global DNS Service.
###### Scope of service
* Global Services(Dont chose region)
  * AWS IAM
  * Amazon Cloud Front
  * AWS route53
  * making a change in service effects everyhwere
* Regional Services(Dont choose availibility zone)
  * Amazon dynomoDB.
  * Amazon Simple Storage Service.
  * Elastic Load Balance.
  * Amazon Virtual Privat Cloud.
* Availability Zone


##### AWS **Identity and Access Management** (Meant for authenticating and authorization against AWS API-- not for OS level or application or database)
* Authentication
* Authorization
* Users
* Groups
* Password Policy
* Multifactor Authenctication
  * What you know (username,password)
  * What you have (like device, netguard)
  * What you are(Biometrics)
  
###### Create User and Groups
* Add Group
  * Define policies (eg can launch EC2 instances)
    * AWS Managed Policies.
    * Custom Policies.
* Add User
  * set password.
  * assign group.
* Access Keys 
  * For API access
##### Amazon Resource Name (ARN)
* Format Pattern
  * arn:partition:service:region:account-id:resourceType/resource
  * arn:partition:service:region:account-id:resourceType:resource
* Examples
  * arn:aws:rds:us-west-2:12345678:db:mysql-db
  * arn:aws:s3:::mybucket/*  (No account id necessary for s3 buckets) (/* means anywhere under mybucket)
  * arn:aws:iam::12345:user/neeraj (No region necessary for global services)
##### Roles
 * We can give roles in code, so that we dont have to specify username,password,etc in our code.
 * For eg EC2(Elastic Compute Cloud) can read files from S3(Simple Storage Service).
##### Fedrated Users
* Existing user need access on AWS without recreating account on AWS

##### MFA Device (Multifactor Authentication
* Virtual MFA
* Physical MFA
#### Resource Policy ????


#### Networking

###### Amazon Virtual Private Network
* Public --
* Private -- Not directly access outside virtual private network
