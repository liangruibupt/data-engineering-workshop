# Lab 6: Ingest and Analysis the Real-time data (Optional)

Real-Time Clickstream Anomaly Detection using Amazon Kinesis and Amazon Kinesis Data Analytics.

## [Real-Time Clickstream Anomaly Detection Kinesis Analytics - Prelab setup](https://aws-dataengineering-day.workshop.aws/300/310-pre-lab.html#real-time-clickstream-anomaly-detection-kinesis-analytics---prelab-setup)

## [Set up the Amazon Kinesis Data Generator](https://aws-dataengineering-day.workshop.aws/300/310-pre-lab.html#set-up-the-amazon-kinesis-data-generator)
1.	Create a EC2 Windows instance to access the Amazon Kinesis Data Generator
    -	AMI: Microsoft Windows Server 2019 Base
    ![kinesis-ec2-1](media/kinesis-ec2-1.png)
    -	Instance type: t2.large
    -	Network: default VPC; 
    -	Subnet: No Preference; 
    -	Auto-assign Public IP: Use Subnet setting (Enable)
    -	IAM Role: TeamRoleInstanceProfile
    ![kinesis-ec2-2](media/kinesis-ec2-2.png)
    -	Storage: Root Volume Size: 50GiB
    ![kinesis-ec2-3](media/kinesis-ec2-3.png)
    -	Tag: Name : KinesisClient
    ![kinesis-ec2-4](media/kinesis-ec2-4.png)
    -	Security Group: Crete new security group; Name ClientSG; Allow 3389 and 443 from 0.0.0.0/0
    ![kinesis-ec2-5](media/kinesis-ec2-5.png)
    -	Key Pair: Select the exsiting key pair Named: ee-default-keypair
    ![kinesis-ec2-6](media/kinesis-ec2-6.png)
    - Wait the EC2 instance become ‘Running’ and Status Check as “2/2 check passed”
    ![kinesis-ec2-7](media/kinesis-ec2-7.png)


2. Go back to ‘https://dashboard.eventengine.run/dashboard’ of your eventengine account, Download the ‘SSH Key’ and Save ‘ee-default-keypair.pem’ to secured place of your desktop
![kinesis-ec2-8](media/kinesis-ec2-8.png)

3. Get the access IP and Username/Password and connect EC2
-	Get the Public IPv4 address
![kinesis-ec2-9](media/kinesis-ec2-9.png)
-	Click ‘Connect’ to get the Username/Password
![kinesis-ec2-10](media/kinesis-ec2-10.png)
-	Browser the ‘ee-default-keypair.pem’ which saved in your desktop，then Click ‘Decrypt Password’
![kinesis-ec2-11](media/kinesis-ec2-11.png)
-	Save the Password for later usage
-	Use the Remote Desktop Client to login the Windows EC2 Instance
![kinesis-ec2-12](media/kinesis-ec2-12.png)

4. Open Kinesis Data Generator
-	Copy KinesisDataGeneratorUrl from CloudFormation Outputs to your Windows Server Web Browser – Suggest you install the Firefox or Chrome 
![kinesis-ec2-13](media/kinesis-ec2-13.png)
-	Then, you can continue the hands-on lab
![kinesis-ec2-14](media/kinesis-ec2-14.png)

## [KINESIS MAIN LAB](https://aws-dataengineering-day.workshop.aws/300/320-main-lab.html)

## [Kinesis Data Analytics for Java Applications (Apache Flink) (Optional)](https://real-time-streaming-with-kinesis.workshop.aws/)