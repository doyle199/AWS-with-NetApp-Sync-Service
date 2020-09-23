# AWS-with-NetApp-Sync-Service
AWS with NetApp Sync Service

The NetApp Cloud Sync services can be utilized to synchronize data backups and archiving to the cloud. The following section will outline how to install the data broker, sync the file server with cloud sync, and create a new EC2 Key Pair.

To install the data broker go to https://cloud.netapp.com/cloud-sync. Go to the Select Source and Target screen. Drag SMB Server to the source.	Drag Amazon S3 to the Target.	Click Continue and click continue again.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/broker.png)

Enter the SMB Server IP.	Click Continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/smb.png)

Enter the SMB Server credentials. Click Continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/creds.png)

To sync your file server with Cloud Sync,	Click on AWS Data Broker. Enter a name. Click Continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/name.png)

It will show that its waiting for AWS.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/con.png)

When the AWS CloudFormation page pops open click Next.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/formation.png)

Select the correct VPC for the Stack name.	Choose the VPC to deploy to. Choose the Subnet to deploy to. Choose the correct EC2 KeyPair. Select True for the assign a public IP address option. Click Next.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/params.png)

If no EC2 KeyPairs show up go to the AWS EC2 Console.	Click on key pairs.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/key.png)

Click on create key pair.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/key2.png)

Name a new keypair. Select the SSH option. Click Create key pair.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/key3.png)

After creating a key pair, if needed, go back to the AWS CloudFormation Dashboard.	Click fill in the information as before and select the new key pair. Click Next.	On the options screen leave everything as default and click Next.	Check the box at the bottom. Click Create stack.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/connect.png)

After about 10 minuets the Cloud Sync webpage will update and show its connected. Click continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/rela.png)

Select Backup_and_Archiving.	Click Continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/arch.png)

Select the correct bucket. Click continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/bucket.png)

Click Continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/bucket1.png)

Click Continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/bucket2.png)

Click Continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/bucket3.png)

Click Continue.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/bucket4.png)

Click Create Relationship.

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/sync7.png)

![alt text](https://github.com/doyle199/AWS-with-NetApp-Sync-Service/blob/master/sync8.png)

