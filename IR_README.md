# aCloudGuru-DynamoDB
Training material from the GitHub repo *acantril/aCloudGuru-DynamoDB*. 

**Some changes were needed in the course material to get them work on the *AWS_Research* account.** 

## Tips:
These are the tips to get examples up and running on your Windows PC against IR's *AWS_Research* account. 

- You need to get IS to allow you access to the EC2 instance used in training. You need to raise an IS request and ask for bidirectional access to the EC2 public IP address via ssh port 22. 
- *LabMachine.json* from the original source will not work as it expects a default VPC configured on AWS account. The *AWS_Research* account does not have a default VPC, hence we needed to point to the specific VPC configured on it. (see *NetworkInterface* bit inside the LabMachine.json file)
- The Windows command-line does not like quotes the way that they're shown in the demos. Use a bash shell like Git or Cygwin.
