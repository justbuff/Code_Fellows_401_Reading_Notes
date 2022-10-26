# Introduction to AWS CloudWatch

Amazon CloudWatch is a service used for real-time monitoring of AWS resources like EC2 instances, EBS, RDS, load balancer, Lambda, Cognito, S3, etc. and also can use for monitoring on-premises resources. CloudWatch is a useful service to collect and track matrices, monitor log files, and set alarms. It automatically provides metrics for CPU utilization, latency and request count. By default, EC2 sends metrics to Amazon CloudWatch and each data point covers the 5 minutes that follow the start time of activity for the instance.

## CloudWatch Events

CloudWatch events allow users to consume a near real-time stream of events like changes to their AWS environment. These event changes can afterword trigger notification services like SNS, SMS, etc. or can trigger other AWS services like Lambda, SSM, or Step function. CloudWatch Events can monitor actions like an AWS service being launched or stopped/terminated and detect when an auto-scale happens. CloudWatch Events consist of Events, Rules, and Targets.

## CloudWatch Agent

CloudWatch agent can be configured on the EC2 instances to send Custom Metrics to CloudWatch. That agent supports multiple operating systems like Amazon Linux, CentOS, Red hat, Windows Server (2008 onwards), Debian, and Ubuntu OS. With the help of IAM role access, the agent can collect live metrics from the server and send custom and detailed data to CloudWatch Dashboard for a better monitoring experience.

## CloudWatch Alarm

CloudWatch alarms can be based on target CloudWatch metrics or the result of a math expression based on CloudWatch metrics. The alarm performs one or multiple actions based on metric values or specified matrices conditions reached over several time periods. 

## CloudWatch Logs

CloudWatch logs help users to access, monitor and store access log files from AWS resources like EC2, Lambda functions, CloudTrail, Route 53, and other sources. CloudWatch logs enable the user to centralize the logs from all systems, applications, and AWS services that you use, in a single, highly scalable service. It offers near real-time monitoring and users can search and filter for specific phrases, values or patterns.



