# Create a Static Website Using Amazon S3

## Introduction

Today I chose this project because I wanted to go back to AWS to be able to compare the cloud providers as cleanly as possible.

## Prerequisite

Utilizing the AWS playground or any of the other virtual area and understanding S3 as a whole.

## Use Case

- Use case/ Benefit of S3 hosting: It scales automatically and there's no need to worry about load balancers or servers, plus It can handle any amount of traffic. 


### Step 1 — Go to [https://github.com/ACloudGuru-Resources/Course-Certified-Solutions-Architect-Associate/tree/master/labs/creating-a-static-website-using-amazon-s3] for the static website code and save both assets.

![Screen Shot 2021-09-23 at 9 55 49 PM](https://user-images.githubusercontent.com/82731990/134606717-80b9ff46-9113-489d-a177-832d2106283f.png)


### Step 2 — Next you want to go and create an S3 bucket. Settings: Accessible to all IP addresses, no versioning enabled, no tags..create. Also copy the ARN of the bucket.

![Screen Shot 2021-09-23 at 9 57 54 PM](https://user-images.githubusercontent.com/82731990/134606846-1d35b47a-5452-46cc-991f-5859a54974fa.png)


### Step 3 — Then you want to enter into your bucket, upload the files saved from github from "add files." After uploading you should get this suceessful upload.

![Screen Shot 2021-09-23 at 10 08 52 PM](https://user-images.githubusercontent.com/82731990/134607780-65c2ddb9-6d7a-4eef-bf6b-6a233f9e364a.png)

### Step 4 — After upload you want to close out of that and click "properties" in your bucket and scroll to the bottom to get to "static website hosting."

![Screen Shot 2021-09-23 at 10 11 59 PM](https://user-images.githubusercontent.com/82731990/134608058-9080aa96-7c58-4e41-9fb7-4f6b1bd644d9.png)
![Screen Shot 2021-09-23 at 10 12 16 PM](https://user-images.githubusercontent.com/82731990/134608090-358a2df3-acf4-44f2-b528-58b8e8130b9d.png)

### Step 5 — Click "edit" for hosting, select "enable" and enter settings like shown. Save changes.

![Screen Shot 2021-09-23 at 10 14 48 PM](https://user-images.githubusercontent.com/82731990/134608246-d37e1097-d345-4bc9-90a4-dd82e2dcf614.png)

### Step 6 — Once saved, scroll back to bottom of bucket page and open link in new tab and it should give you "403 Forbidden" because we haven't allowed permission to the files from the web server. (For showing purposes).

![Screen Shot 2021-09-23 at 10 18 39 PM](https://user-images.githubusercontent.com/82731990/134608533-e63c800d-fdb9-45ca-81ac-2da9f42ddd06.png)

### Step 7 — Now, in your bucket at the top, select "Permissions." Create a bucket policy with the following info. (use your bucket arn).

![Screen Shot 2021-09-23 at 10 36 12 PM](https://user-images.githubusercontent.com/82731990/134609762-279d2422-a4c9-4a94-bf7a-fe531cf93104.png)

### Step 8 — After creating bucket policy, it should show that it is publicly accessible (like shown).

![Screen Shot 2021-09-23 at 10 37 11 PM](https://user-images.githubusercontent.com/82731990/134609969-631f3e83-4578-40ce-811b-6beed3d3d3d2.png)

### Step 9 — Finally, to fact check you can go back to the website from earlier and make sure we do not get the same error code.

![Screen Shot 2021-09-23 at 10 41 11 PM](https://user-images.githubusercontent.com/82731990/134610118-aa49fc78-0cdb-4038-a313-74a4838bbe56.png)

## ☁️ Cloud Outcome

Result: Successfully created a static website in S3. 

## Next Steps

Keep learning!

## Social Proof

[LinkedIn](https://www.linkedin.com/in/stevenwinters24/)
