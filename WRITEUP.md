# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

#### Analyze:
1. Costs:
    + This is a simple application, so it is required to keep the minimum cost as low as possible.
    + This application does not require highly performant computed resources.
2. Scalability:
    + The application needs to be able to adapt to a large number of users and posts at the same time when the number of users is increasing.
3. Availability:
    + The application needs to be available at all times.
    + The application needs to have the ability to backup and restore the data.
    + The application needs to have the ability to respond to client requests as quickly as possible.
#### Chosse:
    + Azure App Service is suitable for my application.
#### Justify my choice:
    + Azure App Service has a lower cost than Azure Virtual Machine and requires less configuration than Azure Virtual Machine.
    + Azure App Service allows you to deploy the application quickly with built-in CI/CD tools without worrying about the underlying infrastructure.
    + Azure App Service has high scalability and built-in autoscaling capabilities that allow it to automatically scale the application based on demand.
    + The Azure App Service has several features:
        - Load Balancing: Prevent overloading requests and ensure the application remains responsive.
        - Automatic Failover: Help the application remain available even in the event of a failure.
        - Backup and Restore: Has built-in backup and restore.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

1. Complexity: If the application becomes more complex and requires the installation of any other libraries or specific software, then Azure Virtual Machine will be suitable for this situation.
2. Performance: If the application requires a highly performant infrastructure like CPU, RAM, etc., then Azure Virtual Machine will be suitable for this situation.
3. Network and security: If the application requires specific network security, Azure Virtual Machine will be suitable for this situation.