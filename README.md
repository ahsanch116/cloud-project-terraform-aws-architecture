# Terraform AWS Architecture Project

This project demonstrates the creation of a simple cloud architecture on AWS using Terraform using code as a structure. The architecture includes a Virtual Private Cloud (VPC) with a public subnet, an Internet Gateway, a route table, and an EC2 instance running Amazon Linux 2023.

## Project Overview

The following resources are created in the `eu-north-1` region:

- **VPC**: A Virtual Private Cloud with a CIDR block of `10.0.0.0/16`.
- **Public Subnet**: A public subnet with a CIDR block of `10.0.1.0/24`.
- **Internet Gateway**: Provides internet access to the resources in the public subnet.
- **Route Table**: Routes all traffic from the public subnet to the Internet Gateway.
- **Security Group**: Allows inbound SSH (port 22) and HTTP (port 80) traffic from any IP address, and allows all outbound traffic.
- **EC2 Instance**: An Amazon Linux 2023 instance (`t4g.micro`) in the public subnet.

## Prerequisites

- AWS account with access keys configured
- Terraform installed on your local machine
- An understanding of basic AWS concepts

## Usage

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/terraform-aws-architecture.git
   cd terraform-aws-architecture
2. **Intialize Terraform**:
   ```bash
   terraform init
3. **Validate the configuration**:
   ```bash
   terraform validate
4. **Apply the configuration**:
   ```bash
   terraform apply
  - Type 'yes' when prompted to create the resources.
5. **Access the EC2 instance**:
    -Once the EC2 instance is created, you can SSH into it using the public IP address.
    -Example:
    ```bash
    ssh ec2-user@<public-ip-address> -i /path/to/your/key.pem
 
## Architecture Diagram
Here’s a simplified diagram of the architecture created by this Terraform configuration:

![Network Diagrams](https://github.com/user-attachments/assets/77133538-08a1-49f5-ac29-6f8f9c626b3f)


## Contact
- Name: Muhammad Ahsan Ijaz
- GitHub: @ahsanch116
- Email: ahsanch116@gmail.com


---

### **Instructions for Usage**
- **Copy this content** into your `README.md` file.
- **Replace** the placeholders like `your-username` and `<public-ip-address>` with the appropriate values.
- **Update the diagram path** in the `Architecture Diagram` section if you upload an image.
  


