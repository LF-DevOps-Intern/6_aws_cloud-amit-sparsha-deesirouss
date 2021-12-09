## AWS Services

### 1. VPC peer from your team’s VPC to next team ie A->B, B->C, …, E->A.
- Allow both direction VPC Traffic.
- Add route to peered VPC in private Route Table.
> https://docs.aws.amazon.com/vpc/latest/peering/vpc-peering-basics.html
## [Peering Connection with ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/tree/cloud-day-3-AWS-Services/3-AWS-Services/Peering%20Connection)


### 2. Create RDS cluster and instance of PostgreSQL.
- Deploy in private subnet.
- In your private EC2. Connect to the RDS Postgresql.
- (Optional) Validate you can connect to another team’s (A->B and B->C) RDS (Peer must be completed)
## [RDS Answer PDF with ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/tree/cloud-day-3-AWS-Services/3-AWS-Services/RDS)

<<<<<<< HEAD
### 3. Install AWS CLIv2 and config lft-training profile.

=======
3. ### Install AWS CLIv2 and config lft-training profile.
## [AWS CLI Answer PDF with ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/tree/cloud-day-3-AWS-Services/3-AWS-Services/Aws%20cli)
>>>>>>> 718ad3891a51a0c5707409145b20a3139030b02d

### 4. Create ECR and upload your Docker image created during Docker assignment Q3.
- Each member must upload an image (in team’s ECR repo) with their name as tag.
## [ECR's Answer PDF with ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-3-AWS-Services/3-AWS-Services/ECR-PDF-with-ScreenShots.pdf)

### 5. Deploy *one* of uploaded image in ECS Fargate.
- Create task definition.
- Deploy in Public Subnet.
- Access via assigned Public IP and your port.
## [Deployment's Answer PDF with ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-3-AWS-Services/3-AWS-Services/Deploy-image-in-ECS-Fargate-PDF-With-ScreenShots.pdf)

### 6. Create a S3 bucket
- Upload Dockerfile of Q4 in the bucket using AWS CLI.
## [S3 bucket's Answer with ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-3-AWS-Services/3-AWS-Services/S3-Bucket-PDF-with%20ScreenShots.pdf)
