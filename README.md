# AWS Three-Tier Architecture with Terraform🚀
![Architecture Diagram](https://raw.githubusercontent.com/waldra/Terraform-three-tier-architecture/main/image/terraform-three-tier.jpg)
## Project Highlights: 
* **Route 53:** Reliable and scalable DNS querying for seamless domain management and high availability.
* **AWS Shield Standard:** Robust DDoS protection to safeguard against malicious traffic, ensuring service continuity.
* **AWS WAF:** Web Application Firewall configured to protect against Cross-Site Scripting (XSS) and SQL Injection attacks, enhancing web application security.
* **CloudFront:** A globally distributed CDN to improve content delivery and latency, ensuring a superior user experience worldwide.
* **VPC** with Three Subnets:
  * **Public Subnet:** For internet-facing services, Application Load Balancer.
  * **Private Subnet:** For App-Tier and Database-Tier instances, ensuring data security.
  * **Database Subnet:** Isolated for MySQL RDS with a read replica, improving read performance under high demand.
* **Internet Gateway and NAT Gateway:** Provided secure internet access for app-tier and database-tier instances while maintaining network isolation.
* **Auto Scaling:** Implemented for both the Web-Tier and Application-Tier to handle traffic spikes dynamically while optimizing costs.
* **MySQL RDS** with Read Replica: Boosted database read performance, ensuring efficient query handling for high-demand scenarios.
## Why Choose Three-Tier Architecture?
* **Scalability:** Each tier can scale independently to meet application demands without over-provisioning resources.
* **Security:** Layered architecture with VPC isolation, WAF, and Shield ensures robust protection at every level.
* **Performance:** CloudFront caching, RDS replication, and auto-scaling maximize performance and minimize latency.
* **Resilience:** High availability and fault tolerance are achieved with distributed components and automated failover mechanisms.
