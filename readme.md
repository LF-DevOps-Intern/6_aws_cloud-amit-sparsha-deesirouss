# AWS Assignment
## 1. Create a VPC with CIDR 10.15.{8*team#}.0/22; no custom subnets.
[VPC answer with Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/main/AWS-VPC.pdf)
- Use us-east-1 (odd) or us-east-2 (even) regions.
## 2. Start a EC2
[EC2 pdf](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/main/EC2%20instance.pdf)
[EC2 SCREENSHOTS](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/tree/main/Snapshots%20EC2)


     - Amazon Linux OS
     - Use t2.micro instance (Free Tire)
     - Attach 10GB General EBS (detachable)
     - Should be publicly accessible
     - Access the the EC2 via SSH
     Firstly, downloaded the key we creted earlier. The changing the mod of the key file using the following command:
          `chmod 400 tead-D-key.pem`
          We accessed the ec2 instance using the following command:
               `ssh -i team-D-key.pem ec2-user@3.12.149.130`
 ![chmod and ssh to ec2-ver](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/main/snapshots/chmod%20and%20ssh%20to%20ec2-user.png)
     - Install OpenVPN package inside the EC2
     We found out that we had to install amazon linux extras and epel dependencies before we get to install openvpn. So we invoked the following command:
          `sudo amazon-linux-extras install epel -y`
          `sudo yum-config-manager --enable epel`
![install amazon estras and epel](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/main/snapshots/installed%20amazon%20extras%20and%20epel.png)
     Now we can install open vpn in our ec2 instance using the following command:
          `sudo yum install openvpn`
![install openvpn](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/main/snapshots/install%20openvpn.png)
Tags:
> Team-Name, Member-1/2/3, Resource Name must include team name too team-1-vpc, team-1-public-subnet
