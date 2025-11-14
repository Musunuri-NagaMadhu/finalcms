# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
*Built-in scalability: App Service can automatically scale up or out based on traffic without manual configuration, making it ideal for fluctuating workloads in the CMS app.

High availability: The platform provides built-in redundancy and load balancing, ensuring consistent uptime without requiring extra setup.

Automated management: OS updates, security patches, runtime updates, and server maintenance are handled by Azure, reducing administrative overhead.

Lower operational cost: Since you don’t manage the underlying infrastructure, App Service reduces both effort and long-term expenses.

Fits the CMS workflow: The CMS app is lightweight and runs well on a PaaS platform, with simple deployment pipelines and no need for specialized configurations.

- *Choose the appropriate solution (VM or App Service) for deploying the app*
Azure App Service is the better deployment option because it offers built-in scalability, high availability, automated management, and lower operational overhead compared to managing a VM. It also reduces cost by eliminating the need to maintain OS updates or server configuration, fitting well with the CMS app’s lightweight workflow. A VM would only become the preferred choice if the app required full OS control, custom runtimes, or specialized background services not supported by App Service.

- *Justify your choice*
Azure App Service is the preferred choice because it provides automatic scaling, high availability, and fully managed infrastructure, which reduces the operational burden compared to maintaining a VM. It is also more cost-efficient since there is no need to manage OS updates or server configuration, making it ideal for the CMS app’s simple and lightweight requirements. A VM would only be necessary if the application required full OS control, custom runtimes, or specialized background services.


### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.*             from the above provided matter give two or three sentences
My decision would change only if the CMS app required capabilities that Azure App Service cannot support, such as full operating system control, custom runtime environments, or specialized background services. If the application evolved to include complex workloads, heavy processing tasks, or custom system-level software, a Virtual Machine would become the more suitable option. In those cases, the flexibility and configurability of a VM would outweigh the convenience of a managed service.
