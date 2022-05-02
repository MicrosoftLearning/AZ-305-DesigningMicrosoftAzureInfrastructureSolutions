---
casestudy:
    title: 'Design a relational storage solution'
    module: 'Relational storage solutions'
---
# Design Relational Storage Case Study

## Requirements

Tailwind Traders is looking to move their existing public website database into Azure, as the website front end is being moved there as well.  The website front end will initially only be deployed in 2 regions for redundancy.  However, it is expected that as traffic increases the website will be replicated to other regions around the world. The database, which you are being asked to migrate, holds the product catalog, and all online orders.  Currently the database runs on a single Microsoft SQL Server Always On availability group on premises.

Primary concerns of Tailwind Traders:

-	**High availability.**  A primary concern for Tailwind Traders is that this database be highly available as it is critical to their business.  Any outages may result in lost sales or customer confidence.

-	**Website performance.**  While the performance of placing orders is normally satisfactory, browsing or searching pages with many items listed is reported as being “sluggish.”

-	**Security.**  Tailwind Traders is very concerned about personal or financial information stored in the database being exposed.  In addition to implementing proper security measures, the security team needs to verify that industry standard best practices are implemented, when possible.


## Tasks

1.	Design the database solution. Your design should include authorization, authentication, pricing, performance, and high availability. 
2.	Diagram what you decide and explain your solution. 

How are you incorporating the Well Architected Framework pillars to produce a high quality, stable, and efficient cloud architecture?
