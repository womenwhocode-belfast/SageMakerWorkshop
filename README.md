# From Zero to AI Hero ft AWS SageMaker 

## Introduction

This workshop is created for Connect NYC Women Who Code Conference in New York. 

### SageMaker 

AI, ML Engineers and Data Scientists need to know more than a Jupyter notebook to delivering production AI services and integrate it with portal or basic web/mobile applications in a flexible and realiable way. 

Inline-style: 
![alt text](https://twitter.com/awscloud/status/996560621922549761/photo/1 "Logo Title Text 1")


## Pre-Requisites

In order to complete the workshop, you'll need an AWS account and full permissions to the following AWS services:
- Create an account [Link]
Can take 24 hours for it to be activated

Basic experience (not mandatory) 
- Train/Test ML Models
- Python (scikit-learn)

In order to complete this workshop you'll need an AWS Account with access to SageMaker and S3. There are resources required by this workshop that are eligible for the AWS free tier if your account is less than 12 months old. 
Check out the the [AWS Free Tier](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc) page for more details.

AWS Credits will be provided on the day. 

## AWS Region

Once you pick which region to use, make sure you use the same region for all servies. Not all regions work with SageMaker so we recommend using [].

## 1. Create S3 bucket

Amazon S3 (Simple Storage Service) is an object storage service that offers industry-leading scalability, data availability, security, and performance. SageMaker uses S3 to store data and model artifacts. 

To begin using S3, sign into the management console

1. Find the [S3](https://aws.amazon.com/s3/) Service from the management console
2. Click on **+Create Bucket** 
3. Provide a name for your bucket (This must be a globally unique name)
4. Select Region, make sure you use the same one thoughout this workshop
5. Click **Create**
6. Your bucket should then appear, click it
7. Download data from this repo and upload to S3 bucket

You can now see that your bucket has been created. You can set many configurations and permissions for your bucket. S3 provides easy to use management features so you can organise your data and configure finely-tuned access controls to meet your specific business, organizational needs. 

## 2. SageMaker 

Navigate back to AWS management services and search for SageMaker, click on this and it will navigate you to the SageMaker console. 

Note: Make sure you are in the correct region 

As you can see from first glance, SageMaker provides many features. The first page it takes you to us a dashboard that shows the user an overview and recent activity. On the left hand side you will see a menu with many different SageMaker features such as labeling, notebook, training and inference. 

### 3. Create Notebook Instance

1. First we want to create a notebook instance, navigate to this option on the menu 
2. At the top right, click **Create Notebook Instance**
3. Provide the instane name and type. E.g. wwcode-smworkshop and select ml.t2.medium [instance](https://aws.amazon.com/sagemaker/pricing/instance-types/)
4. For Permissions and encryption, select **create a new role** in the IAM role dropdown menu. In the pop-up modal, select Specific S3 buckets and type in the name of your bucket and a comma followed by gdelt-open-data and then click 'create role'.
5. After this, you should be navigated back to the create notebook instance page and you should see a green box saying 'success....'
6. Select **Enable**, to give users root access to the notebook. 
7. Click **Create Notebook Instance**

There are many other optional features that you can set up such as VPC, Tags and Git Repo. For this tutorial, we will be cloning the git repo in the notebook instance terminal. 

8. Wait for the server status to change to **InService**. This may take several minutes.
9. Click **Open Jupyter**, You will now see the Jupyter homepage for your notebook instance.


### 4. Clone Project to Notebook Instance

1. On the Jupyter notebook homepage at the top right, click on **New** which will open a dropdown menu. Click **Terminal**. This will then open a Jupyter Notebook Terminal!
2. Type [CD] **git clone https://github.com/womenwhocode-belfast/SageMakerWorkshop.git** to clone this project into jupyter notebook. 

There is another way to do this [..] 

For this workshop, we are using the breast cancer dataset. 

## 5. Data Cleaning

To find out more about the data cleaning for this dataset, please go to [] Notebook. 

In Jupyter Notebook, open file [..] 

## 6. Data Training








