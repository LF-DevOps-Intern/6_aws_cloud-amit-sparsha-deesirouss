## Logs & Alerts

### 1. Validate your email address in SES.
### 2. Create SNS topic.
- Add subscription as Protocol Email, and endpoint your Email Address.
### [SES and SNS (Assignment 1 and 2) with ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-5-Logs-and-Alerts/5-Logs-and-Alerts/AWS-LOGS(1%20and%202).pdf)

### 3. Create Event Bridge rule to monitor EC2 state change events. Set above created SNS topic as target.
### [Event Bridge Answer in PDF with ScreenShots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-5-Logs-and-Alerts/5-Logs-and-Alerts/Event-Bridge-PDF-with%20ScreenShots.pdf)

### 4. (Optional)
- Create standard SQS.
- Add this SQS as target in above created Event Bridge rule (in addition to existing SNS)
- Add lambda trigger in SQL to sendEmail lambda function.
### [Task's Answer in PDF with Screenshots](https://github.com/LF-DevOps-Intern/6_aws_cloud-amit-sparsha-deesirouss/blob/cloud-day-5-Logs-and-Alerts/5-Logs-and-Alerts/Lambda-Fubction-SQS-Triggered-PDF%20with%20Screenshots.pdf)
