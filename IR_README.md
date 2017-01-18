# aCloudGuru-DynamoDB
This project is forked from GitHub repo *acantril/aCloudGuru-DynamoDB*. It was customised to run course exercises on IR’s AWS_Research account.

## Summary

The instructor is very knowledgeable and he explains database and DynamoDB related concepts very well. This course was designed for beginners as well as for people who have experience in databases and want to learn DynamoDB. 

At times the course flow was a bit tedious and slow moving, as most of us are not alien to databases. You may want to skip certain sections that you know well and run videos with a speed faster than x1.0. I don’t recommend skipping modules all together though, as they are related.

This course is very lengthy, although 20 hours was projected for it, you need to double that at least (1 man week). You can use time more effectively if you follow my tips given below.

I would recommend this course to anyone who wants to learn advanced DynamoDB concepts. However finding 40 hours is obviously not easy.

## Tips:
These are the tips to get examples up and running on your environment against IR's *AWS_Research* account. 

### Platforms
- This course relies on setting up a platform in order to run commands and scripts against AWS DynamoDB.   
- The course gives 4 options to run AWS CLI commands and Python scripts, Windows, OSX, Linux and EC2.
- You can save time to focus on setting up one platform. 
- If you have a fast Internet connection skip EC2, don’t waste your time setting it up. I’ll explain why at the end.

### Windows
- The Windows command-line does not like quotes the way that they're shown in the demos. Use a bash shell like Git or Cygwin.
- Running Python scripts on Windows reliably and getting a sensible output was not always possible. Some scripts refused to run. Some of them ran but the horizontal progress output was scrolling vertically.

### OSX
- The OSX environment worked best. Python on OSX worked like a charm and performed excellently. 

### EC2 (avoid)
- The instructor did not mention why we are setting up EC2 upfront. It wasn’t clear EC2 was an alternative platform to run Python scripts until midway through.      
- If you decide to use EC2, You need to get IS to allow you access to the EC2 instance used in training. You need to raise an IS request and ask for bidirectional access to the EC2 public IP address via ssh port 22. 
- If you decide to use EC2, the file *LabMachine.json* from the original source will not work as it expects a default VPC configured on AWS account. The *AWS_Research* account does not have a default VPC, hence I needed to point to the specific VPC configured on it (see *NetworkInterface* bit inside the LabMachine.json file).
- Using EC2 as command portal was problematic. I had to re-create EC2 instance a few times due to various issues, every time I did that I needed to create a separate IS request, as EC2 public IP address changed for every instance. 
- EC2 can only be helpful if you have a slow Internet connection, then you will need to go through the trouble of setting it up because it will perform faster than your local machine. If you have a fast Internet connection you can avoid using EC2.
