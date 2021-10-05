# Use Terraform to Create an EKS Deployment

## Introduction

Today, the goal is to start learning Kubernetes at a higher level, which is why today's topic is such.

## Prerequisite

For this project its recommended to have an understanding of Kubernetes. You will also need to create a terraform account and sign up with aws to utilize free tier and playground.

## Use Case

- AWS EKS can be used for a multitude of different use cases, such as reliably running your web applications and having them scale automatically across multiple availability zones, as well as fully integrate with other AWS services like load balancers

## Cloud Research

- My research included videos and readings of Terraform and EKS.

## Try yourself

https://learn.acloud.guru/handson/24cb7511-50f6-4cfb-8c24-396d2634282e

### Step 1 — To start we're going to log into the lab environment and then log into the CLI and list the directories.

![Screen Shot 2021-10-04 at 10 12 18 PM](https://user-images.githubusercontent.com/82731990/135949601-c23f8361-c7f5-4c8e-b1b7-8134a13be970.png)


### Step 2 — Next, cd into the "eks" directory and list to see all files. 

![Screen Shot 2021-10-04 at 10 22 24 PM](https://user-images.githubusercontent.com/82731990/135950408-5c15d990-c0ee-4465-9c84-1ad93b5d723f.png)


### Step 3 — vim into all files to review them individually. (:q!) to quit/ go back.
#### Provider info
![Screen Shot 2021-10-04 at 10 30 42 PM](https://user-images.githubusercontent.com/82731990/135951096-e15849f4-4198-4586-990a-4350d59d734c.png)
#### Resources and worker groups
![Screen Shot 2021-10-04 at 10 32 19 PM](https://user-images.githubusercontent.com/82731990/135951193-fb3a9c9b-fc32-482c-9a7f-6635dd6fe76b.png)
#### Security groups
![Screen Shot 2021-10-04 at 10 33 02 PM](https://user-images.githubusercontent.com/82731990/135951251-4aff9771-9de5-4d39-9aca-b17c18f5d5d6.png)
#### VPC info
![Screen Shot 2021-10-04 at 10 33 33 PM](https://user-images.githubusercontent.com/82731990/135951292-9dfd27c4-5ac0-4951-b792-f5d24465d063.png)
#### Versions
![Screen Shot 2021-10-04 at 10 34 35 PM](https://user-images.githubusercontent.com/82731990/135951367-cc1dcb49-2ceb-4c78-bb01-b1db386521b6.png)
#### Output info
![Screen Shot 2021-10-04 at 10 39 55 PM](https://user-images.githubusercontent.com/82731990/135951754-f404114e-b526-4cb2-b27f-45fe347328d9.png)

### Step 4 - Initial the working directory (terraform init) and check for errors (terraform plan).
![Screen Shot 2021-10-04 at 10 43 49 PM](https://user-images.githubusercontent.com/82731990/135952140-007b0121-dba0-4d16-af05-67a473e6946b.png)
![Screen Shot 2021-10-04 at 10 46 28 PM](https://user-images.githubusercontent.com/82731990/135952250-acacfd33-7944-4979-adb7-098d661cf79c.png)

### Step 5 - Deploy the cluster (terraform apply).
![Screen Shot 2021-10-04 at 11 08 57 PM](https://user-images.githubusercontent.com/82731990/135953945-f07af520-6157-4a49-8765-4ca65010bf06.png)

### Step 6 - Configure the kubctl to talk to clusters. Confirm clusters are up and running like shown.
![Screen Shot 2021-10-04 at 11 12 07 PM](https://user-images.githubusercontent.com/82731990/135954208-5b345b61-f9fa-4ab4-b033-7a2ec6b162fb.png)

### Step 7 - Now, we're downloading the file that containg the configuration for the NGINX deployment.
![Screen Shot 2021-10-04 at 11 16 43 PM](https://user-images.githubusercontent.com/82731990/135954574-ad153c83-d8a9-4978-81a9-432225cade8b.png)

### Step 8 - Next deploy the NGINX pods.
![Screen Shot 2021-10-04 at 11 20 32 PM](https://user-images.githubusercontent.com/82731990/135954866-68623a6a-9631-4a27-92ab-bdc5a848329a.png)

### Step 9 - Finally we're going to clean it all up and destroy the eks cluster. (terraform destroy). You can also verify it has been destroyed (terraform destroy).
![Screen Shot 2021-10-04 at 11 26 54 PM](https://user-images.githubusercontent.com/82731990/135955320-529e966e-c4bd-499b-ab03-2b8ec1f543cb.png)

## ☁️ Cloud Outcome

✍️ Successfully created and AWS EKS cluster using Terraform and added to configuration by adding a 2pod NGINX deployment and destroyed the cluster.

## Next Steps

✍️ Continue learning Kubernetes and Dockers.

## Social Proof

[LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:6843941959430656000/)
