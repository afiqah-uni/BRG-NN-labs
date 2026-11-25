# Topic 7: Provisioning and Securing a Cloud VM (AWS EC2)

## Setting Up My Cloud Server

For this activity, I used Amazon Web Services (AWS) to provision an EC2 virtual machine. I selected Ubuntu Server 24.04 LTS as the operating system and used a `t3.micro` instance with an 8 GiB gp3 storage volume.

After launching the instance, I connected to it remotely from my MacBook using SSH:

`ssh -i ~/Downloads/ubuntu-key.pem ubuntu@13.210.238.56`

This allowed me to access and manage the Ubuntu server through the terminal without needing to use its desktop environment.

## Security Group Configuration and Troubleshooting

An important part of setting up the server was configuring its security group. I used inbound rules to control which network traffic could reach the instance. SSH access used TCP port 22, while HTTP traffic used TCP port 80 so that the web server could be accessed.

I encountered an SSH connection timeout during the activity, even though the EC2 instance was running. After checking the security group, I changed the SSH source setting to "My IP". This allowed me to connect successfully.

## Reflection

This activity helped me understand how cloud virtual machines can be created and accessed remotely. I also learned that launching a server is not enough; its network access must be configured carefully. Restricting SSH access to my own IP address helped me understand the importance of limiting remote access.

These skills are relevant to cloud administrators and DevOps engineers, who need to provision servers, manage remote access and configure network security when maintaining cloud infrastructure.
