
# Design a network infrastructure solution  

## Requirements

As the Tailwind Traders Enterprise IT team prepares to define the strategy to migrate some of company’s workloads to Azure, it must identify the required networking components and design a network infrastructure necessary to support them. Considering the global scope of its operations, Tailwind Traders will be using multiple Azure regions to host its applications. Most of these applications have dependencies on infrastructure and data services, which will also reside in Azure. Internal applications migrated to Azure must remain accessible to Tailwind Traders users. Internet-facing applications migrated to Azure must remain accessible to any external customer. 

To put together the initial networking design, the Tailwind Traders Enterprise IT team chose two key applications, which are representative of the most common categories of workloads that are expected to be migrated to Azure.  

### Design - Product catalog enterprise application

![Product catalog architecture](media/catalog.png)

- An internet-facing, Windows-based two-tier .NET Core-based web app providing access to the product catalog, hosted in a SQL Server Always On Availability Group database. This application is categorized as mission-critical, with availability SLA of 99.99%, 10-minute RPO and 2-hour RTO. 

-	Business leads emphasize the importance of the optimal customer experience when accessing internet-facing apps, so it is critical that the time it takes to load web pages and download static content is minimized. Similarly, a failure of individual servers hosting web app components and their dependencies should have negligible impact on the web app availability perceived by customers. While it’s understood that a regional failure might introduce some interruption to existing web sessions, the failover to a disaster recovery site should be automatic.

- To take advantage of benefits offered by Azure PaaS services, the Enterprise IT team decided to implement the database of the product catalog enterprise application by using Azure SQL Database. 

- The Tailwind Traders Information Security and Risk teams require all communication between Azure VMs and PaaS services that are part of the same application must travel via Azure backbone, rather than via a public endpoint of the PaaS services. 

## Tasks - Product catalog enterprise application

1. Design a two-tier network solution for the Product Catalog. Where appropriate your design could include Azure Front Door, WAF, Azure Firewall, and Azure Load Balancer. Your networking components should be grouped into virtual networks and network security groups should be considered. Be prepared to explain why you chose each component of the design. 

How are you incorporating the Well Architected Framework pillars to produce a high quality, stable, and efficient cloud architecture?

