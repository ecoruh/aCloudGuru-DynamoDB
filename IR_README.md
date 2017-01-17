# aCloudGuru-DynamoDB
This project is forked from GitHub repo *acantril/aCloudGuru-DynamoDB*. It was customised to run course exercises on IR’s AWS_Research account.

## Tips:
These are the tips to get examples up and running on your Windows PC against IR's *AWS_Research* account. 

- The course is very lengthy, although 20 hours was projected for it, you need to double that at least (1 man week).
- The course gives 4 options to run AWS CLI commands and Python scripts, Windows, OSX, Linux and EC2.
- The Windows command-line does not like quotes the way that they're shown in the demos. Use a bash shell like Git or Cygwin.
- Running Python scripts on Windows reliably and getting a sensible output was not possible. Some scripts refused to run. Some of them ran but the horizontal progress output was scrolling vertically.
- If you decide to use EC2, You need to get IS to allow you access to the EC2 instance used in training. You need to raise an IS request and ask for bidirectional access to the EC2 public IP address via ssh port 22. 
- If you decide to use EC2, the file *LabMachine.json* from the original source will not work as it expects a default VPC configured on AWS account. The *AWS_Research* account does not have a default VPC, hence I needed to point to the specific VPC configured on it (see *NetworkInterface* bit inside the LabMachine.json file).
- Using EC2 as command portal was problematic. I had to re-create EC2 instance a few times due to various issues, every time I did that I needed to create a separate IS request, as EC2 public IP address changed for every instance. EC2 command execution performance was also the worst among others. My two cents; avoid using EC2.
- The OSX environment worked best. Python on OSX worked like a charm and performed excellently.
- The instructor is very knowledgeable and he explains concepts very well. I think our developers may feel a bit overqualified in some areas, so they may need to skip certain sections and run videos with a speed faster than x1.0.
- I would recommend this course to anyone who wants to learn advanced DynamoDB concepts. However finding 40 hours is obviously the problem.
