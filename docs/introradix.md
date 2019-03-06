## What is Omnia Radix

- Platform-as-a-Service (PaaS)
- Hosting web applications and apis
- Infrastructure as code
- Continuous integration and continuous deployment
- Monitoring
- Developers focus on delivering functionality


Note:
Omnia Radix is a Platform-as-a-Service, where developers can define resources it requires to host their applications through code. Much of the details around network, VMs, OS, etc is taken care of by the platform. 

Compare to Azure and ARM templates (hard to get right)

Integrate with a code repository so that it can continuously build, test, and deploy applications. For instance, Radix can react to a git push event, automatically start a new build, and push it to the test environment, ready to be tested by users.

Radix also provides monitoring for applications. There are default metrics (e.g. request latency, http failure rate), but you can also output custom metrics from your code. Track things that are important for your application: uploaded file size, number of results found, or user preferences. Radix collects and monitors the data.
