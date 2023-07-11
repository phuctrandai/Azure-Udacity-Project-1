# Write-up

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

#### Analyze:
1. Costs:
    * Azure Virtual Machine (VM) is more expensive than Azure App Service.
    * VM come with many pricing options: Pay as you go, Azure savings plan for compute, Reserved instances, and Spot. Meanwhile, Azure App Service comes with Pay as you go, Azure savings plan for compute, and Reservations.
    * VM has two tiers, Basic and Standard; pricing is based on the size and configuration, such as CPU, memory, and disk storage. Azure App Service has tiers ranging from Basic to Premium, and the pricing is based on that range, with each tier offering different levels of performance and pricing.
    * For example, with tier Basic, the OS Ubuntu, 1 CPU core, 1.75 GB of RAM, and 40 GB of storage, the VM cost is about 23$ per month, but the Azure App Service cost is about 13$ per month.

2. Scalability:
    * VM can have higher scalability by grouping multiple instances into a scale set. We can configure it automatically to increase or decrease the number of instances, or manually add or remove instances as needed.
    * App Service has good built-in autoscaling capabilities with vertical and horizontal scaling based on demand.
    * VM has a scale limit: The platform image is 1000 nodes per scale set, and the custom image is 600 nodes per scale set. And Azure App Service has a scale limit of 30 instances, compared to 100 with the App Service Environment.
  
3. Availability:
    * VM can offer high availability by grouping multiple instances into a scale set or configuring them in an availability set. This helps ensure that the application remains available even if one or more VM instances fail.
    * App Service has built-in high-availability features such as autoscaling, load balancing, and geo-replication. App Service also has deployment slots for testing, staging, and production; they can be swapped to reduce downtime during deployment.

#### Choose the solution:
    * Azure App Service is suitable for this application for the following reasons:
        + This is a simple application and does not require a highly performant computed resource.
        + This is a small application, so it needs to be deployed as fast as possible and does not require complex setup steps.
    * In the feature, if the application changes based on the following reasons, I would like to change to VM:
        1. Complexity: If the application becomes more complex and requires the installation of any other libraries or specific software, then Azure Virtual Machine will be suitable for this situation.
        2. Performance: If the application requires a highly performant infrastructure like CPU, RAM, etc., then Azure Virtual Machine will be suitable for this situation.
        3. Network and security: If the application requires specific network security, Azure Virtual Machine will be suitable for this situation.