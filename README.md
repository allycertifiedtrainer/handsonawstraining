# Simple Steps to Lower Amazon AWS Usage Costs

EC2:
Use spot instances for back-end processes (non-UI, background processes, and so on). Spot instances have the lowest per-hour costs when compared to On-demand, Reserved, and well Spot instances. If your application requirements are consistent and long-term, utilizing Reserved instances saves you money. Reserved instance pricing is up to 75% cheaper than on-demand instance rates.

When configuring auto-scaling, scale up rapidly and gently. Keep in mind that each stop and start (even if the instance was only running for a single second) counts as one full hour for Amazon AWS billing reasons. Instead of larger EC2 sizes, use smaller EC2 sizes with Autoscaling.
Remove any new EBS volumes or snapshots.
Elastic IP: Delete Elastic IP when it is no longer assigned to any instance. Unassigned Elastic IP addresses are charged.

### S3 (Simple Storage Service):
Use simple storage service (s3) life cycle management of objects and, where applicable, move things to Glacier. For easily reproducible objects (such as image thumbnails), use the "Reduced Redundancy" storage class, which has lower charges than "standard" storage.
In addition to storage, S3 charges for both bandwidth and amount of HTTP requests. For example, one 50MB item retrieval cost is smaller than two 25MB object retrievals. Consolidate objects (e.g., log files) before putting them in S3 to decrease S3 access (HTTP) costs.
[AWS Training and Certification] helps you build and validate your skills so you can get more out of the cloud.

[//]: # (Any comments)
[AWS Training and Certification]:<https://www.netcomlearning.com/amazon-web-services-training/vendor/104/?advid=1356>

CloudFront - Amazon Content Delivery Network (CDN): Use Billing Alerts to receive notifications when charges surpass specific thresholds. This aids in preventing AWS billing surprises.

CloudWatch may be used to track the consumption of all AWS resources. CloudWatch offers AWS resource use information that you may use to improve a specific AWS resource.
For example, you may be utilizing an Elastic Computing (EC2) setup that isn't actually necessary, or auto-scaling EC2 instances aren't enough during high-demand situations.

[AWS Training and Certification] can help you be more effective and do more in the cloud.

[//]: # (Any comments)
[AWS Training and Certification]:<https://www.netcomlearning.com/vendors/aws-training.phtml?advid=1356>

Even if you have completed all of the above procedures, you should consider using Amazon's AWS Trusted Advisor. This functionality is free to use and available in the Amazon AWS administration Console. This tool examines your AWS account for possible security vulnerabilities, cost-saving opportunities, and system performance and dependability. Trusted Advisor is offered in a free edition as well as business and enterprise support levels.
