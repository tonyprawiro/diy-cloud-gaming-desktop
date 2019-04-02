# diy-cloud-gaming-desktop

Proof of concept of using AWS GPU instance and Spot-block to build a powerful and cost-effective Steam-powered cloud gaming desktop.

https://aws.amazon.com/blogs/aws/build-3d-streaming-applications-with-ec2s-new-g2-instance-type/

# Disclaimer

This guide is intended for people who already have decent experience of using AWS and understand what they are doing.

I will not be responsible for any issues or cost incurred as a result of following (or not following) the steps in this document. Use this guide at your own risk.

# Pre-Requisites

## Choose the Closest AWS Region to You

Latency and bandwidth will be one of the key constraints of any cloud-based desktop. You would want to choose an AWS region closest to where you will be using your cloud gaming desktop.

After logging in to your AWS account, choose the region at the top right corner.

<img src="images/region.png" />

# (Optional) Create a KeyPair

# Step : Create a Security Group

<img src="images/security-group.png" width="600" />

# Step : Create an EBS Volume for Storing Game Data

<img src="images/ebs-volume.png" width="600" />

# (Recommended) Step : Allocate an Elastic IP Address

<img src="images/elastic-ip.png" width="600" />

# Step : Start a g2.2xlarge Instance for Imaging Purpose

<img src="images/os.png" width="600" />

<img src="images/instance-type.png" width="600" />

<img src="images/storage.png" width="600" />

<img src="images/instance-tags.png" width="600" />

<img src="images/security-group.png" width="600" />

<img src="images/launch.png" width="600" />

# Step : Associate the Elastic IP to the Instance

<img src="images/associate-eip.png" width="600" />

# Step : Attach the EBS Volume to the Instance

<img src="images/attach-ebs.png" width="600" />

# Step : Decrypt Administrator Password

<img src="images/decrypt-windows-password.png" width="600" />

# Step : Configure the Instance

## Connect to the Instance via RDP

<img src="images/connect-rdp.png" width="600" />

## (Recommended) Install Mozilla Firefox

<img src="images/getfirefox.png" width="600" />

## Prepare the EBS Volume Drive

diskmgmt.msc

<img src="images/disk-online.png" width="600" />

<img src="images/disk-initialize.png" width="600" /> MBR partition style

<img src="images/disk-newvolume.png" width="600" />

Max size

Assign drive letter D

Format as NTFS (Quick Format)

## Install NVIDIA Graphics Driver

https://docs.aws.amazon.com/AWSEC2/latest/WindowsGuide/install-nvidia-driver-windows.html

<img src="images/download-driver.png" width="600" />

<img src="images/download-driver2.png" width="600" />

Restart

## Disable Microsoft Basic Display Adapter

Open Device Manager

<img src="images/disable-basic-display-driver.png" width="600" />

## Start and Enable Windows Audio Service

<img src="images/windows-audio-service.png" width="600" />

## (Optional) Install NotePad++

<img src="images/notepadplusplus.png" width="600" />

## Change Documents Folder Location

<img src="images/move-documents.png" width="600" />

## Download and Install Steam

<img src="images/install-steam.png" width="600" />

## Download and Install the Game



# Step : Stop the Instance and Detach the EBS Volume

# Step : Create a Golder Master Image

# How to Use

## (Optional) Step : Check the Current Spot Pricing

## Step : Send a Spot Request

## (Optional) Step : Check the Spot Request Fulfillment

## Step : Attach the EBS Volume

## (Optional) Step : Associate the Elastic IP Address

## 

## Step : Connect to the Instance via RDP

## Step : 

# Cost Calculation
