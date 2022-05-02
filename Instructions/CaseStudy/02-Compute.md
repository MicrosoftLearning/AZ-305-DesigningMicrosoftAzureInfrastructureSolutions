---
casestudy:
    title: 'Design a compute solution'
    module: 'Compute solutions'
---

# Design a compute solution

## Requirements

Tailwind Traders would like to migrate their product catalog application to the cloud. This application has a traditional 3-tier configuration using SQL Server as the data store. The IT team hopes you can help modernize the application. They have provided this diagram and several areas that could be improved. 

![compute architecture](media/compute.png)

* The frontend application is a .NET core-based web app. During peak periods 1750 customers visit the website each hour. 

* The application runs on IIS web servers in a front-end tier. This tier handles all customer requests for purchasing products. During the latest holiday sale, the front-end servers reached their performance limits and page loads were lengthy. The IT team has considered adding more servers, but during off hours the servers are often idle.

* The middle tier hosts the business logic that processes customer requests. These requests are often for help desk support. Support requests are queued and lately the wait times have been very long. Customers are offered email rather than wait for a representative. But many customers seem frustrated and are disconnecting rather than wait. Customer requests are 75-125 per hour. 

* The back-end tier uses SQL Server database to store customer orders. Currently, the back-end database servers are performing well.

* While high availability is a concern, due to legal requirements the company must keep all the resources in a single region.

## Tasks

* **Front-end tier**. Which Azure compute service would you recommend for the front-end tier? Explain why you decided on your solution. 

* **Middle tier**. Which Azure compute service would you recommend for the middle tier? Explain why you decided on your solution. 

How are you incorporating the Well Architected Framework pillars to produce a high quality, stable, and efficient cloud architecture?
