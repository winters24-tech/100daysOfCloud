![Screenshot](https://user-images.githubusercontent.com/82731990/133858389-3b2f8904-a7bf-42e6-b80f-819056974ab8.png)

# Creating a Lambda Function Using The AWS Console

## Introduction

Today I chose creating a Lambda function just wanting to learn the biggest serverless compute service. This allows me to see how to utilize the Lambda service and functions and this particular lab was based on a url checker to see how a website would return the status code of the site.

## Prerequisite

Before starting this lab it would best to know what Lambda is and the many functions and abilities it work with.

## Use Case

- Lambda functions is useful for everyday projects, the Lambda function is the foundational principle of Lambda. You can configure your functions using the Lambda console, Lambda API, AWS CloudFormation or AWS SAM. You create code for the function and upload the code using a deployment package. Lambda invokes the function when an event occurs. Lambda runs multiple instances of your function in parallel, governed by concurrency and scaling limits.


## Cloud Research

- Below you will get to see the steps I followed to create the function and capture the status code and at the end viewing the log stream from CloudWatch.

### Step 1 — Creating the Lambda function using "author from scratch" and using "node.js"

![Screenshot](https://user-images.githubusercontent.com/82731990/133858502-4a9112a5-1eb5-4c9a-bada-3fb8b078039b.png)

### Step 2 — Showing the function successfully created.

![Screenshot](https://user-images.githubusercontent.com/82731990/133858723-6ffffb33-3052-41e1-b3ae-3b688a2008d5.png)

### Step 3 — Creating the test event to capture the status code of the website.

![Screenshot](https://user-images.githubusercontent.com/82731990/133858739-64b02dcb-499b-4abe-b7f8-788f59583e13.png)

### Step 4 — After creating the test event you can see that test came back with the status code of "200" meaning the site is up running actively.

![Screenshot](https://user-images.githubusercontent.com/82731990/133858772-c2bc53be-310b-4a38-a5d4-032017622ee6.png)

### Step 5 — Checking the CloudWatch Logs for the function, viewing the log streams.

![Screenshot](https://user-images.githubusercontent.com/82731990/133858949-2133065b-7e44-4581-95be-a4564e7771a6.png)

## ☁️ Cloud Outcome

Results: I successfully created a function and verified the site was running by showing status code 200. I also messed around with different websites, even fake
ones to see the change of the status. 

## Next Steps

Next for me would be to learn how to perform more functions using Lambda. I believe it would have a huge use case for DevOps teams which is my goal.

## Social Proof

[LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:6843941959430656000/)
