# Creating Amazon S3 Buckets, Managing Objects, and Enabling Versioning

## Introduction

Today I am extending some learning in S3, for day 9 I created a static website and now I will be doing a little more in the actual buckets.

## Prerequisite

- Must own an amazon account to perform in the virtual labs.
- Have an understanding of the projected topic.

## Use Case

- 🖼️ (Show-Me) Create an graphic or diagram that illustrate the use-case of how this knowledge could be applied to real-world project
- ✍️ (Show-Me) Explain in one or two sentences the use case

## Cloud Research

- ✍️ Document your trial and errors. Share what you tried to learn and understand about the cloud topic or while completing micro-project.
- 🖼️ Show as many screenshot as possible so others can experience in your cloud research.

### Step 1 — First you want to go in and create your S3 bucket.

![Screen Shot 2021-09-24 at 9 35 06 PM](https://user-images.githubusercontent.com/82731990/134753526-e6b61881-56ba-4988-83a3-ae48cde06d61.png)

### Step 1.5 — In this scenario we're going to add tags and create a 2nd bucket the same way. (1 will be public and 1 private).

![Screen Shot 2021-09-24 at 9 37 47 PM](https://user-images.githubusercontent.com/82731990/134753635-b334d972-b13a-499a-847f-dec3f0dd7a87.png)

### Step 2 — After viewing and seeing that the "public" bucket we created is not actually public, we will go to the "permissions" tab to update it.
- Note: You can actually make it public when creating the bucket.

![Screen Shot 2021-09-24 at 9 43 29 PM](https://user-images.githubusercontent.com/82731990/134753804-2a69e49c-4e2d-415a-b169-c48a2ade7949.png)
![Screen Shot 2021-09-24 at 9 44 40 PM](https://user-images.githubusercontent.com/82731990/134753809-5d7225da-1e94-42c5-a0f8-e8d719659faa.png)

### Step 3 — Back in the S3 buckets overview, after the update, you can see the public is now open to public objects and the private is still blocking access.

![Screen Shot 2021-09-24 at 9 49 38 PM](https://user-images.githubusercontent.com/82731990/134753886-e14e8bf5-1ea9-41aa-b6a5-1bc16b310446.png)

### Step 4 — Next, we'll go in to our public bucket and add a file (keep default configuration), enter the file uploaded and select the object URL.

![Screen Shot 2021-09-24 at 9 54 59 PM](https://user-images.githubusercontent.com/82731990/134754148-bd67d420-34da-4a2f-85b2-462ecb0ab7f8.png)
![Screen Shot 2021-09-24 at 9 58 57 PM](https://user-images.githubusercontent.com/82731990/134754159-6add879d-0852-437e-bbf9-7635fee0df88.png)

### Step 5 — When entering the object URL page, you should recieve this "access denied" page.

![Screen Shot 2021-09-24 at 9 59 42 PM](https://user-images.githubusercontent.com/82731990/134754191-2de1c697-7816-41f2-a165-8f26bda03c38.png)

### Step 6 — The reason we have been denied is because, even though the bucket is public, we need to make the object public as well. [Security reasons].
- Showed is the way to perform making the file public.

![Screen Shot 2021-09-24 at 10 01 22 PM](https://user-images.githubusercontent.com/82731990/134754246-111eb0b1-c498-487b-b50e-799981bb1554.png)

### Step 7 — For showing purposes, you will now see that after the object is made public it is now accessing on the web.

![Screen Shot 2021-09-24 at 10 15 28 PM](https://user-images.githubusercontent.com/82731990/134754541-e849e792-cc42-469b-b0ee-c66fa41ec97f.png)

### Step 8 — Next, we'll do the same steps with our private bucket, also using another file (if possible). This shows the private object url created and webpage showing the same "access denied" screen.

![Screen Shot 2021-09-24 at 10 24 08 PM](https://user-images.githubusercontent.com/82731990/134754775-b0e02d6e-a02d-44ef-a76c-f95242d7e420.png)
![Screen Shot 2021-09-24 at 10 24 17 PM](https://user-images.githubusercontent.com/82731990/134754778-ed122ade-6311-4ac6-8fee-28f1ec45bc84.png)

### Step 9 — Attempting to make the object in the private bucket public, it will decline it due to bucket being private. [Like shown].

![Screen Shot 2021-09-24 at 10 26 05 PM](https://user-images.githubusercontent.com/82731990/134754830-26955dc5-5862-49a7-9949-bfb3ece18205.png)

### Step 10 — Now to quickly show you how to enable versioning..I went into the public bucket, uploaded the 'updated' file and to make it accessbile you will need to make it public just like before with the objects.
- Shown is the bucket showing the versions of the object.

![Screen Shot 2021-09-24 at 10 37 43 PM](https://user-images.githubusercontent.com/82731990/134755153-fa7c49b0-c73d-4294-9d61-3d0a23e6f9a9.png)

### Step 11 — After enabling versions in the bucket, select the "object url" of the new version of the uploaded object and it should allow you to access it in the web. (Like shown).

![Screen Shot 2021-09-24 at 10 46 22 PM](https://user-images.githubusercontent.com/82731990/134755361-8cb430d7-a47e-49ba-8712-33e5e0b2ffde.png)

## ☁️ Cloud Outcome

Results: Successfully completed project.

## Next Steps

Never stop progressing and building knowledge.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)
