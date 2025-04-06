# Project-ID-101-Three-Tier-Architecture_v1.0
Highly available three tier architecture of AWS

🔹 Project Highlights
🌐 Global DNS with Route 53: Efficient routing of user requests to the nearest CloudFront edge location for reduced latency and improved performance.

⚡ Content Delivery with CloudFront: Caches static assets at edge locations, improving load times and reducing origin load.

🌍 External Load Balancer (ALB): Distributes incoming internet traffic across auto-scaled web servers in multiple availability zones.

📈 Auto Scaling Group: Automatically scales the Web Tier based on demand to ensure high availability and cost optimization.

🖥️ Web Tier in Private Subnets: Hosts secure and scalable web servers behind the external load balancer.

🔒 Internal Load Balancer (ALB): Handles communication between the Web Tier and Application Tier in a secure and isolated manner.

🧠 Application Tier: Hosts business logic in private subnets, shielded from public internet exposure.

🗃️ Database Tier: Stores application data in a Multi-AZ RDS setup for durability and fault tolerance.

🚪 VPC Gateway Endpoint for S3: Secure and private access to Amazon S3 without traversing the public internet.

📂 Elastic File System (EFS): Shared storage for EC2 instances across tiers, allowing concurrent access from multiple Availability Zones.
