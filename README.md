# Project-ID-101-Three-Tier-Architecture_v1.0
Highly available three tier architecture of AWS

🔹 ProjectThree tier Application – Key Highlights

🌐 Global DNS with Route 53: Efficiently routes user traffic to the nearest CloudFront edge location for reduced latency.

⚡ Content Delivery with CloudFront: Serves cached static content from edge locations to enhance speed and availability.

🌍 External Load Balancer (ALB): Distributes incoming internet traffic across web servers in multiple AZs for high availability.

📈 Auto Scaling Group: Dynamically scales the Web Tier based on traffic and performance metrics for cost-efficiency.

🖥️ Web Tier in Private Subnets: Hosts web servers securely behind the external load balancer with no direct internet access.

🔒 Internal Load Balancer (ALB): Handles secure communication between Web Tier and App Tier.

🧠 Application Tier: Processes business logic in a secured environment within private subnets.

🗃️ Database Tier: Uses Amazon RDS in Multi-AZ mode for high availability, automated backups, and failover support.

📂 Elastic File System (EFS): Provides scalable, shared storage for EC2 instances across multiple AZs.

🚪 VPC Gateway Endpoint (S3): Enables private connectivity to Amazon S3 without exposing traffic to the public internet.

📊 CloudWatch Monitoring: Tracks application and infrastructure metrics (CPU, memory, etc.) with custom alarms for performance insights.

📩 SNS Notifications: Sends real-time alerts for CloudWatch alarms and application events to email/SMS for proactive incident response.
