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
