# Working with Basic Regular Expressions

## Introduction

I chose today's project of continuing Linux learning, we'll be reading some text files and redirecting some output (output that we'll decide on using regular expressions) to other text files.

## Prerequisite

Knowing Linux commands and Bash scripting.

## Try yourself

Free tutorial: https://learn.acloud.guru/handson/71c92ea2-300d-4610-a75a-9f6ab2d8771d

### Step 1 — Locate HTTP Services. 
- We'll start with using the command "grep ^http[^x] /etc/services > ~/http-services.txt" and then checking it in the new file system.

![Screen Shot 2021-10-08 at 9 00 05 PM](https://user-images.githubusercontent.com/82731990/136638308-df7bb272-8ff3-4758-9dcf-e70ac1d95666.png)

### Step 2 — Locate LDAP Services. Additionally checking the file system as well.
- We want to find all of the lines in /etc/services that start with ldap. 
- The fifth character can be any alphanumeric character, but the sixth character can not be an a. We'll dump the output into ~/lpic1-ldap.txt

![Screen Shot 2021-10-08 at 9 04 40 PM](https://user-images.githubusercontent.com/82731990/136638427-d75baee0-fa3e-465a-9dcf-2613224aa624.png)

### Step 3 — Refine the HTTP Results. We want to read the ~/http-services.txt file that we created earlier, and just look at lines that don't end with the word service. This grep command will do it:

![Screen Shot 2021-10-08 at 9 08 16 PM](https://user-images.githubusercontent.com/82731990/136638528-cc2f95ed-39ed-47ac-9153-3c5155edd6c8.png)

## ☁️ Cloud Outcome

Successfully got the information from each output in the file system.

## Next Steps

Finish up Linux learning strong

## Social Proof

[LinkedIn](https://www.linkedin.com/in/stevenwinters24/)
