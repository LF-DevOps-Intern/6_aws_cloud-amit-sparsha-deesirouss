# VPC Components
- Terminate previously created EC2
> All task are in continuation of yesterday’s setup. Use same VPC and tag convention for all resources.
## Flow Logs
- #### (Optional) Enable VPC Flow Logs via CloudWatch Log.
### [Flow-Log Answer With ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-2-vpc-components/2-VPC-Components/VPC-Flow-Logs/VPC-Flow-Logs.pdf)

## Subnets
- #### Create 3 subnets in each AZ to be used as public.
- #### Create 3 subnets in each AZ to be used as private.
### [Subnets Answer with Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-2-vpc-components/2-VPC-Components/Subnets/Subnets-Pub%26Pvt.pdf)

## Route Tables
- #### Create Public Route Table and associate public subnets.
- #### Create Private Route Table and associate private subnets.
### [Route Tables Answer with Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-2-vpc-components/2-VPC-Components/Route-Tables/Route-Tables-Pub%26Pvt.pdf)

## Internet Gateway
- #### Create Internet Gateway and attach its route in public route table.
### [Internet Gateway Answer](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-2-vpc-components/2-VPC-Components/Internet%20Gateway/Internet%20gateway.pdf)
### [Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/tree/cloud-day-2-vpc-components/2-VPC-Components/S3%20Endpoints/Screenshots)

## NAT
- #### Create NAT (and EIP for it) and attach its route in private route table.
### [NAT Answer](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-2-vpc-components/2-VPC-Components/NAT/NAT.pdf)
### [Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/tree/cloud-day-2-vpc-components/2-VPC-Components/NAT/Screenshots)

## S3 Endpoint
- #### Create S3 VPC Endpoint and add its route to both public and private Route tables.
### [S3 Endpoint](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-2-vpc-components/2-VPC-Components/S3%20Endpoints/S3%20EndPoint.pdf)
### [Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/tree/cloud-day-2-vpc-components/2-VPC-Components/S3%20Endpoints/Screenshots)

### Create EC2 inside Public Subnet
- Allow SSH ingress traffic for your own IPs only.
- Spin up simple http server @ 9099 port and verify it is accessible from public.
- Install and Setup OpenVPN Server, open ports required to use it for these CIDR ranges 27,43,45,72,103,110,112,124,139,150,163,202.0.0.0/8 and your own IPs.
- (Optional) Create a OpenVPN Client with Split tunnel to use that Server Help1, Help2, Help3
### [EC2 inside Public Subnet](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-2-vpc-components/2-VPC-Components/Ec2%20inside%20public%20subnet/EC2%20Inside%20Public%20Subnet.pdf)
### [Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/tree/cloud-day-2-vpc-components/2-VPC-Components/Ec2%20inside%20public%20subnet/Screenshots)

### Create another EC2 inside Private Subnet
- Only allow inbound traffic within VPC
- Install PostgreSQL and open its port to VPC only.
- Connect to PostgreSQL from above created EC2.
- (Optional) Connect to PostgreSQL server from your local PC (hint: use OpenVPN connection)
### [EC2 Pvt tasks with Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-2-vpc-components/2-VPC-Components/EC2-Inside-Pvt-Subnet/EC2-private.pdf)
