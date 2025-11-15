# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
   
 1.cost-
    app service -Pay-as-you-go, optimized for web apps only and No need to manage OS, patching, or updates → lower operational cost.
    vm -Pay for complete VM compute time, even when idle and You must maintain OS updates & security patches → higher admin and maintenance costs.
2.scalability-
    app service -Auto-scaling available out-of-the-box that is 1.Scale out by adding instances,2.Scale up by upgrading plan.Zero downtime during scaling.
    vm -Scaling must be manually configured via:VM Scale Sets (extra configuration work).Scaling may involve downtime unless configured very carefully.
3.availability-
    app service -Built-in 99.95% availability SLA (depending on plan).Multiple deployment slots (staging, production) improve availability during updates.Easy backup & restore options.
    vm -SLA depends on VM configuration.Requires:Availability Sets or Availability Zones for high availability.You must manually configure:Failover,Load balancing,Health monitoring.
4.workflow-
    app service -Seamless CI/CD with GitHub Actions,Azure DevOps,Zip deploy,Docker container deploy.Faster & simpler deployment workflow.
    vm -CI/CD is possible but requires custom setup.More flexibility for custom environments but slow setup & heavy maintenance.
  
- *Choose the appropriate solution (VM or App Service) for deploying the app*
  
   Azure App Service is the preferred choice because it delivers a fully managed, cost-efficient, and highly available environment tailored specifically for web applications. Its built-in scalability and seamless CI/CD support allow the CMS to run smoothly without the need to manage servers or infrastructure. This makes it a simpler, faster, and more reliable deployment solution than a Virtual Machine.so,azure app service is best for deploying the Flask CMS app.

- *Justify your choice*

Azure App Service is the best choice because it handles all server, OS, and security management automatically, reducing operational effort and cost. It provides built-in scaling, high availability, and seamless CI/CD, ensuring the Flask CMS app runs efficiently under varying workloads. These advantages make it a simpler, more reliable, and more optimized deployment option than a Virtual Machine.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.*             from the above provided matter give two or three sentences
Flask CMS app fits perfectly into a standard web-hosting model,so i think there is no need to change the decision from App Service.
