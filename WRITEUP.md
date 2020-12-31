# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*


VMs offer different configurations (CPU, RAM, storage) and we can choose what software to install on it.  This gives a great deal of flexibility.  The VMs can be grouped to provide high availability and scaling.  The VM will most likely be more expensive, and it will require more work to deploy the app because we have to manage the software on the server.

App Services offer different pricing based on Number of Apps, Disk Space, Number of Instances.  It has high availability and auto-scaling.  The App Service will most likely be cheaper and it will have a more simple workflow because the developer does not have to spend time configuring the software on the server.

For this project I would choose the App Service.  The app uses Python, which is supported by App Services.  A VM is not necessary, because the application is a simple web app, and the VM would just be hosting the application.  There's no real reason why the developer should be concerned with setting up the web server, firewall, etc on the VM.


### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 


I would use a VM if:

1. The application required a programming language that was not supported by App Services
2. The application required specific third party software
3. The application was no longer an HTTP based service
