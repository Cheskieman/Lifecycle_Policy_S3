# Configure different lifecycle policies for specific items in an S3 Bucket

## Full Step by Step Guide with snapshots to both describe and illustrate how to set different lifecycle policies for items placed inside an S3 bucket.

### This project will display how to set different lifecycle policies provided by AWS for items contained in an S3 bucket, including: 

*Create a S3 Bucket

*Create a Lifecycle Policy to move objects to the S3 intelligent tier after 60 days

*Create a Lifecycle Policy to move objects to S3 Glacier after 90 days

*Create a Lifecycle Policy to delete objects after 120 days


#### Instructions on how to create an S3 Bucket and individual lifecycle policies

**CREATE A LIFECYCLE POLICY TO MOVE OBJECTS TO S3 INTELLIGENT TIER AFTER 60 DAYS (STEP BY STEP)**

*Select S3 (from AWS search tab)
    <p align="center">  
  <img src="resources/S3 Select from AWSSEARCHbarS3photo.png" alt="Select S3 from AWS " width="900" />  
</p>  
*Select Create Bucket
  <p align="center">  
  <img src="S3CreateBuckettabselectphoto.png" alt="Select Create Bucket" width="900" />  
</p>  
*In the "General Configuration" section, give your Bucket a name
    <p align="center">  
  <img src="S3BucketNamephoto.png" alt="S3Bucket Name" width="900" />  
</p> 
*Scroll to the bottom and select Create Bucket
  <p align="center">  
  <img src="S3CreateBucketonCreateBucketpagephoto.png" alt="Select Create Bucket at Bottom" width="900" />  
</p>  
*Click on the S3 bucket you just created
    <p align="center">  
  <img src="S3click oncreatedbucketphoto.png" alt="Click on recently created bucket" width="900" />  
</p>  
*Select the Management tab from the top
  <p align="center">  
  <img src="s3 management tabphoto.png" alt="Click on Management tab in S3" width="900" />  
</p>  
*Select Create Lifecycle Rule from the "Lifecycle Configuration" section
  <p align="center">  
  <img src="Create Lifecycle Polocies.png" alt="Select Lifecycle Rule button" width="900" />  
</p>  
*Create a lifecycle rule name and prefix under the "Lifecycle rule configuration" section
  <p align="center">  
  <img src="s3lifecyclerulenameandprefixphoto.png" alt="Select Lifecycle Rule name and Prefix" width="900" />  
</p>  
*Select Transition Current versions of objects.... as well as select the acknowledgement in the "Lifecycle rule actions" section
  <p align="center">  
  <img src="Lifecycle rule actions transition current versions of objects between storage classes.png" alt=" Select Transition current version of object between storage classes" width="900" />  
</p>  
*Select Intelligent Tiering under Choose Storage Class Transitions and 60 for Days after object creation under "Transition current versions of objects between storage classes" section 
  <p align="center">  
  <img src="S3 S3 Intelligent-Tiering Archive configurations creatre configurationphoto.png" alt="Select Intelligient Tiering & 60 days" width="900" />  
</p>  
*Click Create Rule at the bottom
  <p align="center">  
  <img src="Create Rule bottom.png" alt="Create Rule" width="900" />  
</p>  
*Click on the S3 bucket you just created. Select the Properties tab from the top
  <p align="center">  
  <img src="S3 Select Propertiesoptionphoto.png" alt="Select Properties tab " width="900" />  
</p>  
*Scroll down to where it says S3 Intelligent-Tiering Archive configurations and choose Configuration
  <p align="center">  
  <img src="Sel" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Give your configuration a name, select a Prefix and set a tag under the "Archive configuration settings" section 
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Click Create on Bottom.
<p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  

**CREATE A LIFECYCLE POLICY TO MOVE OBJECTS TO S3 GLACIER AFTER 90 DAYS (STEP BY STEP)**


*Select Create Lifecycle Rule from the "Lifecycle Configuration" section
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Create a lifecycle rule name and prefix under "Lifecycle rule configuration"
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Select "Transition current versions of objects"
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Check the acknowledgement box
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Under "Lifecycle rule actions," choose "Transition current versions of objects between storage classes"
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Select "Glacier Instant Retrieval" as the storage class
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Set transition to "90 days after object creation"
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Click "Create Rule"
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
 **CREATE A LIFECYCLE POLICY TO DELETE OBJECTS AFTER 120 DAYS**

*Select Create Lifecycle Rule from the "Lifecycle Configuration" section
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Create a lifecycle rule name and prefix under "Lifecycle rule configuration"
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
*Select Expire Current versions of objects
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
* Select 120 for Days after object creation
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  
* Select the Create Rule button at the bottom
  <p align="center">  
  <img src="Selectr ec2 from AWS searchbar.png" alt="Select EC2 from AWS Searchbar" width="900" />  
</p>  




##### Contribution Policy

This project is not accepting external contributions, including pull requests or feature requests.

It serves as a personal archive of my learning journey in applying foundational concepts in software development and version control. Active development is not ongoing, and external changes will not be integrated.

Thank you for your understanding.
