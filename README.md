# aws-vpc-project

Create a secure VPC that you can use for servers in a Production Environment.

To improve resiliency, you deploy the servers in two Availability Zones, by using an Auto Scaling group and an Application Load Balancer. For additional security, you deploy the servers in private subnets. The servers receive requests through the load balancer. The servers can connect to the internet by using a NAT gateway. To improve resiliency, you deploy the NAT gateway in both Availability Zones.

Before we start get some idea about following concepts:
1. VPC: 
VPC is a virtual network that you create in the cloud. It allows you to have your own private section of the internet, just like having your own network within a larger network. 
Within this VPC, you can create and manage various resources, such as servers, databases, and storage.
Think of it as having your own little "internet" within the bigger internet. This virtual network is completely isolated from other users' networks, so your data and applications are secure and protected.

2. Auto Scaling Group: 
An Auto Scaling Group (ASG) in AWS is a feature that helps automatically scale the number of EC2 instances (virtual machines) up or down based on the demand or defined conditions, ensuring that your application maintains performance and availability.

3. Load Balancer:
A Load Balancer in AWS distributes incoming traffic across multiple targets (e.g., EC2 instances, containers, IP addresses) to ensure high availability, reliability, and fault tolerance.

4. Target Group:
A Target Group in AWS is a configuration resource used with Elastic Load Balancers (ELB) to route incoming traffic to specific targets, such as EC2 instances, containers (ECS tasks), Lambda functions, or IP addresses. The Target Group determines how requests are distributed and how the health of each target is checked.

5. Bastion Host: 
Bastion Host (also known as a "jump box") is a security measure in a cloud or network environment that provides secure access to private or isolated resources (such as EC2 instances in private subnets) via a publicly accessible host. It acts as a secure entry point, typically allowing administrators to SSH or RDP into other instances that are not directly accessible from the internet.

![20](https://github.com/user-attachments/assets/773ed293-2a44-47d5-abbd-7865251e3add)

![21](https://github.com/user-attachments/assets/4297b8be-83d9-4584-8ee7-775089fabfbf)
![22](https://github.com/user-attachments/assets/202fc453-5de8-46e2-953f-23178e714223)
![23](https://github.com/user-attachments/assets/2cbbd8e1-7264-41f2-a8a5-8466383bb583)
![24](https://github.com/user-attachments/assets/938b448b-5c90-415e-a34b-5f67d9101767)
![25](https://github.com/user-attachments/assets/6c870754-5fe7-40ea-8db5-4e31e5030f12)
![26](https://github.com/user-attachments/assets/20fc626c-3f56-4266-a788-2df770c43a0e)
![27](https://github.com/user-attachments/assets/3f447fa1-3390-4ded-aa58-c683e20a7521)
![28](https://github.com/user-attachments/assets/bb6b3961-a48a-4299-87e7-f2964f71f511)


