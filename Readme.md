# A script that runs on the Cloudtrail logs in Elasticsearch
# Determines, whether the role credentials setup on an EC2 instance have been compromised
# Require access to Elasticsearch cluster
# Requires a role or AWS Access key with IAM permission to: 
	ec2:DescribeNetworkInterfaces
	ec2:DescribeAddresses
# Point the script to the CloudTrail Index in Elasticsearch cluster to execute it
# Setup an incoming webhook for a Slack channel and pass that to the script
# Read '-h' options of the script for execution examples