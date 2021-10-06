# Set Up a WordPress Site Using EC2 and RDS

## Introduction

Hi, welcome to day 12 of 100days of cloud. Today I'm going to learn more EC2 and RDS to set up a WordPress.

## Prerequisite

Having access to a free tier account of AWS and utilize the labs.

## Use Case

- Amazon RDS and EC2 will help you to build a database in a secure environment, supports high-performance applications, and are highly scalable.

### Step 1 — Create an RDS; utilizing standard create, MySQL, free tier.

![Screen Shot 2021-10-05 at 10 52 24 PM](https://user-images.githubusercontent.com/82731990/136133491-3b727ff2-6bc9-48eb-987b-0daec19f37c0.png)

### Step 2 — While RDS is being deployed, let's prepare our EC2 instance and select your instance and connect to the server.

![Screen Shot 2021-10-05 at 10 59 31 PM](https://user-images.githubusercontent.com/82731990/136133808-451e7fc9-9491-4028-8d30-bdaa6b8c491d.png)

### Step 3 — In the instance terminal we're going to install Apache and Dependencies with code like shown.

![Screen Shot 2021-10-05 at 11 03 27 PM](https://user-images.githubusercontent.com/82731990/136134144-f5bff22b-9e0e-4e52-8035-c622e8222122.png)

### Step 4 — Next, we'll go into the new /var/www directory with code (cd /var/www) and list the content of the directory with (ls).

![Screen Shot 2021-10-05 at 11 07 20 PM](https://user-images.githubusercontent.com/82731990/136134451-f38ab4ce-13ee-4bae-8620-e1e5e33a36d4.png)

### Step 5 — Followed by adding wordpress to the /var/www directory and listing the content to verify it has been added (like pictured).

![Screen Shot 2021-10-05 at 11 08 30 PM](https://user-images.githubusercontent.com/82731990/136134537-4531d959-ca35-4153-9c10-e3838becf3c3.png)

### Step 6 — Now, we're going to move into WordPress directory and move the Apache configuration file into "/etc/apache2/sites-enabled/" to enable the WordPress website to work from /var/www/wordpress:   using sudo mv 000-default.conf /etc/apache2/sites-enabled/.  and finally restarting the Apache 2 configuration.

![Screen Shot 2021-10-05 at 11 28 53 PM](https://user-images.githubusercontent.com/82731990/136136325-35488830-9590-4aad-a16a-d9cfdeee7da7.png)

### Step 7 — In this step we'll click the wordpress database. In the Connectivity & security tab, under Endpoint, copy the endpoint provided into your clipboard. Return to your terminal. Change the line define('DB_HOST', 'localhost'); to read: define('DB_HOST', ' <'INSERT ENDPOINT HERE>'); Save and exit by pressing Control + X, followed by Y, and hitting Enter.
  
![Screen Shot 2021-10-05 at 11 34 12 PM](https://user-images.githubusercontent.com/82731990/136136668-1d2c7b95-933d-45b1-9f8f-9d08aefa3ddb.png)
![Screen Shot 2021-10-05 at 11 34 43 PM](https://user-images.githubusercontent.com/82731990/136136677-58c5b383-f146-4995-a54b-c173259d06c6.png)


### Step 8 — Back to your EC2 instance in your security groups, select the non-default group and change inbound rules. For the new rule, from the Type dropdown menu, select MYSQL/Aurora. In the dropdown menu to the right of the Source column for the new rule, find and select the non-default security group.

![Screen Shot 2021-10-05 at 11 26 00 PM](https://user-images.githubusercontent.com/82731990/136135979-90de5008-e35b-45d4-9754-df394336bc90.png)

### Step 9 — Next, in the terminal open up the public IP address in a new webpage and it should take you to the WordPress installation page.
![Screen Shot 2021-10-05 at 11 36 14 PM](https://user-images.githubusercontent.com/82731990/136136842-e7534e48-9b6e-429b-b656-4bc79e02f451.png)
![Screen Shot 2021-10-05 at 11 37 19 PM](https://user-images.githubusercontent.com/82731990/136136864-3d61b92a-a334-48f1-b0b5-09256ede8b30.png)

### Step 10 - After setting up credentials in the installation page you should be able to login and view your WordPress dashboard.
![Screen Shot 2021-10-05 at 11 38 36 PM](https://user-images.githubusercontent.com/82731990/136137049-067dad1b-9049-489d-90a1-9dcc4f44cd7c.png)

### Step 11 - Finally view your created website.
![Screen Shot 2021-10-05 at 11 40 51 PM](https://user-images.githubusercontent.com/82731990/136137159-030d119c-649b-4cd0-88a9-8386fc535977.png)

## ☁️ Cloud Outcome

Sucessfully configured RDS and EC2 to visit my WordPress site!

## Next Steps

Continue learning!

## Social Proof

[LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:6843941959430656000/)
