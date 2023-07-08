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
    * VM requires more steps to configure and deploy the application, while App Service allows us to quickly deploy with built-in CI/CD tools without worrying about the underlying infrastructure.

2. Scalability:
    * VM can have higher scalability by grouping multiple instances into a scale set. We can configure it automatically to increase or decrease the number of instances, or manually add or remove instances as needed.
    * App Service has good built-in autoscaling capabilities with vertical and horizontal scaling based on demand.
  
3. Availability:
    * VM can offer high availability by grouping multiple instances into a scale set or configuring them in an availability set.
    * App Service has built-in high-availability features such as autoscaling, load balancing, and geo-replication. App Service also has deployment slots for testing, staging, and production; they can be swapped to reduce downtime during deployment.

#### Choose the solution:
    * Azure App Service is suitable for this application for the following reasons:
        + This is a simple application and does not require a highly performant computed resource.
        + This is a small application, so it needs to be deployed as fast as possible and does not require complex setup steps.
    * In the feature, if the application changes based on the following reasons, I would like to change to VM:
        1. Complexity: If the application becomes more complex and requires the installation of any other libraries or specific software, then Azure Virtual Machine will be suitable for this situation.
        2. Performance: If the application requires a highly performant infrastructure like CPU, RAM, etc., then Azure Virtual Machine will be suitable for this situation.
        3. Network and security: If the application requires specific network security, Azure Virtual Machine will be suitable for this situation.