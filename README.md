# Create-and-Configure-a-Virtual-Private-Cloud-VPC-with-Subnets
To learn how cloud networking works by creating a Virtual Private Cloud (VPC) with public and private subnets, and enabling controlled internet access. This task teaches the backbone of secure cloud architecture and how resources are isolated and protected in the cloud.


AWS Free Tier (Preferred) – VPC, Subnets, Route Tables, Internet Gateway, Security Groups

 (also free-tier eligible)

📦 Deliverables:

✅ Screenshot of VPC dashboard showing subnets
✅ Screenshot of route table configuration
✅ Short description: CIDR range, number of subnets, region, and whether internet access is enabled

🧭 Detailed Mini Guide (Step-by-Step):1️⃣ Login to Cloud Console

Use AWS or Google Cloud (Free Tier account)

Open VPC Dashboard

2️⃣ Create a Virtual Private Cloud

Click Create VPC

Choose IPv4 CIDR block: 10.0.0.0/16
(This defines your private cloud network)

3️⃣ Create Subnets

Create Public Subnet:

CIDR: 10.0.1.0/24

Enable auto-assign public IP

Create Private Subnet:

CIDR: 10.0.2.0/24

Disable auto-assign public IP

4️⃣ Create and Attach an Internet Gateway (IGW)

Navigate to Internet Gateways → Create

Attach it to your VPC (enables internet access for public subnet)

5️⃣ Route Table Configuration

Create a Public Route Table

Add route: 0.0.0.0/0 → Internet Gateway

Associate with Public Subnet

Create a Private Route Table

No internet route (remains isolated)

6️⃣ Verify

Go to VPC → Subnets

Confirm:

Public subnet has internet access

Private subnet is isolated

7️⃣ Save and Document

Take screenshots and note:

VPC name

CIDR block

Subnet details

Routing configuration
