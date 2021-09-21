![Screen Shot 2021-09-20 at 10 26 59 PM](https://user-images.githubusercontent.com/82731990/134102612-a65f778e-0443-4f9a-acd2-472d01dd73c5.png)

# Creating a virtual network via the Azure Portal

## Introduction

Today was learning more of the fundamentals in Azure, so I chose to create a virtual network via the Azure Portal.

## Prerequisite

You require need an Azure subscription to perform these steps. If you don't have one you can create one by following the steps outlined on the Create your Azure free account today webpage.

## Use Case

- 🖼️ (Show-Me) Create an graphic or diagram that illustrate the use-case of how this knowledge could be applied to real-world project
- ✍️ (Show-Me) Explain in one or two sentences the use case

## Cloud Research

- ✍️ Document your trial and errors. Share what you tried to learn and understand about the cloud topic or while completing micro-project.
- 🖼️ Show as many screenshot as possible so others can experience in your cloud research.

## Try yourself

They do have a free mini tutorial to show you how to perform this task as well via the Microsoft Azure account.

### Step 1 — Choose Create a resource in the upper left-hand corner of the Azure portal, then select Networking > Virtual network. Then complete the rest of the configuration settings to create the virtual network.

![Screen Shot 2021-09-20 at 10 40 43 PM](https://user-images.githubusercontent.com/82731990/134103629-1c034ca8-334b-4c55-8d4b-f18d2eccb78d.png)


### Step 2 — Verify the creation of the virtual network by going to the newly created resource group and viewing the virtual network is present, located in the East US region.

![Screen Shot 2021-09-20 at 10 42 22 PM](https://user-images.githubusercontent.com/82731990/134103769-0b79b529-98cf-475c-a2ba-049ad1dc5fef.png)


### Step 3 — Next, we'll create a VM in the network.

![Screen Shot 2021-09-20 at 10 48 08 PM](https://user-images.githubusercontent.com/82731990/134104192-9ef6f62d-0694-46c4-87e7-38554c4ff353.png)

### Step 4 — After verifying VM is created (like shown), create another VM the same way.

![Screen Shot 2021-09-20 at 10 56 37 PM](https://user-images.githubusercontent.com/82731990/134104872-c4ae7f80-5bd6-4905-b7a4-d710062ea050.png)


### Step 5 — Once you have both VMs created, let's go ahead and connect to the first one created by locating it in the resource group. Select it and connect.

![Screen Shot 2021-09-20 at 11 09 25 PM](https://user-images.githubusercontent.com/82731990/134105894-82f2cd69-2d14-4331-a719-8bba1557bbea.png)

### Step 6 — In the Connect to virtual machine page, keep the default options to connect by DNS name over port 3389 and click Download RDP File. Open the downloaded RDP file and click Connect when prompted and then use your created login info.

![Screen Shot 2021-09-20 at 11 15 54 PM](https://user-images.githubusercontent.com/82731990/134106352-100d6604-6ae5-43eb-bf2c-07e6a25be030.png) ![Screen Shot 2021-09-20 at 11 16 38 PM](https://user-images.githubusercontent.com/82731990/134106412-6ec120c5-8184-4116-b79c-8e0a5dd888d2.png)

### Step 7 — Once again my Mac is old and outdated so I will use screenshots from a Windows cpu. But next you want to open up PowerShell and run as "administrator" running the comman [ping VM2-100DaysOfCloud(or whatever your 2nd VM name is)].

- PS: The ping will fail because ping uses the Internet Control Message Protocol (ICMP). By default, ICMP isn't allowed through the Windows firewall.

![Screen Shot 2021-09-20 at 11 37 53 PM](https://user-images.githubusercontent.com/82731990/134107892-3d661e27-94c3-43b2-8477-e0cf4eaee029.png)

### Step 8 - To allow vm2 to ping vm1 enter the below command which will allow ICMP inbound through the Windows firewall:

- New-NetFirewallRule –DisplayName “Allow ICMPv4-In” –Protocol ICMPv4

![Screen Shot 2021-09-20 at 11 40 10 PM](https://user-images.githubusercontent.com/82731990/134108078-20e0a4c1-5958-4884-bbb8-e9f48314df21.png)

### Step 9 - Now we'll connect to VM2 the same way we did for VM1, using rdp. i.e. open vm2 properties and click the Connect button to download and then connect vis RDP. Open up PowerShell and run command: "ping vm1"

![Screen Shot 2021-09-20 at 11 42 49 PM](https://user-images.githubusercontent.com/82731990/134108313-78ad1fa4-5100-42cc-a6c7-fda04b9f8e9e.png)

### Step 10 - This is the end! You should now be able to ping the vm1 virtual machine successfully, because ICMP has been configured to be allowed through the Windows firewall on the vm1 virtual machine in an earlier step.

![Screen Shot 2021-09-20 at 11 45 44 PM](https://user-images.githubusercontent.com/82731990/134108517-964f881c-185d-408a-83a9-08384c1ccbc7.png)

## ☁️ Cloud Outcome

✍️ (Result) Describe your personal outcome, and lessons learned.

## Next Steps

✍️ Describe what you think you think you want to do next.

## Social Proof

✍️ Show that you shared your process on Twitter or LinkedIn

[link](link)
