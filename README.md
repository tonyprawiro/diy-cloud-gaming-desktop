# diy-cloud-gaming-desktop

Proof of concept of using AWS GPU instance and Spot-block to build a powerful and cost-effective Steam-powered cloud gaming desktop.

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

<img src="images/security-group.png" />

# Step : Create an EBS Volume for Storing Game Data

<img src="images/ebs-volume.png" />

# (Recommended) Step : Allocate an Elastic IP Address

<img src="images/elastic-ip.png" />

# Step : Start a g2.2xlarge Instance for Imaging Purpose

<img src="images/os.png" />

<img src="images/instance-type.png" />

<img src="images/storage.png" />

<img src="images/instance-tags.png" />

<img src="images/security-group.png" />

<img src="images/launch.png" width="480" />

# Step : Associate the Elastic IP to the Instance

<img src="images/associate-eip.png" />

# Step : Attach the EBS Volume to the Instance

# Step : Configure the Instance

## (Recommended) Install Mozilla Firefox

## Initialize the EBS Volume Drive

## Create NTFS Partition on the Drive

## Configure and Assign Drive Letter to the Partition

## Install NVIDIA Graphics Driver

## Enable Windows Audio Service

## (Optional) Install NotePad++

## Change Documents Folder Location

## Download and Install Steam

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