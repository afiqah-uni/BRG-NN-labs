# Topic 3 – Managing and Controlling Linux Services

## Introduction

In this session, I learned about Linux services and how they operate in the background to support different functions of a server. A service is a program that runs in the background and provides specific functionality, while a daemon is a type of background process that usually operates without direct user interaction.

I learned that managing services is an important part of server administration because services need to be installed, started, monitored and checked to ensure that the server is functioning properly.

## Tools and Commands Used

During this practical activity, I used an AWS EC2 Ubuntu server and its terminal to manage and test the Apache web server.

Some of the commands I used were:

- `sudo apt install apache2` – installs the Apache web server.
- `sudo systemctl status apache2` – checks the current status of Apache.
- `systemctl list-units --type=service` – displays the services managed by systemd.
- `sudo apache2ctl configtest` – checks Apache configuration files for syntax errors.
- `curl -I http://localhost` – tests whether Apache responds to an HTTP request locally.

## My Practical Experience

For this practical activity, I used my AWS EC2 Ubuntu server, which I had previously set up. I installed Apache using the command `sudo apt install apache2`. Apache is a web server that allows a server to host and deliver web pages through HTTP.

After installing Apache, I checked whether the service was running using `sudo systemctl status apache2`. The output showed that Apache was active and running. I also noticed that its status was enabled, meaning it was configured to start automatically when the server boots.

Next, I used `systemctl list-units --type=service` to view the services running on my Ubuntu server. I noticed that Apache appeared as `apache2.service`, alongside other services such as SSH, cron and rsyslog. This helped me understand that a Linux server runs multiple background services, each responsible for different tasks.

I also checked the Apache configuration using `sudo apache2ctl configtest`. The output displayed `Syntax OK`, which confirmed that there were no syntax errors in the Apache configuration files.

## Testing the Apache Web Server

After checking the service status and configuration, I tested whether Apache could respond to HTTP requests. I first used `curl -I http://localhost` from my AWS terminal. The output returned `HTTP/1.1 200 OK`, showing that Apache was responding successfully to requests made locally on the server.

I then tested the server from my Mac terminal using its public IP address. The response also returned `HTTP/1.1 200 OK`, confirming that the web server could be accessed externally.

Finally, I tested my DuckDNS domain, `afiqahaws.duckdns.org`, using another curl command. This also returned `HTTP/1.1 200 OK`. Through this test, I understood how a domain name could be used to access a web server instead of having to remember its numerical IP address.

## Challenges and Reflection

One challenge I encountered was when I initially tried to connect to my AWS server through SSH. The connection timed out because the SSH security group rule needed to allow access from my current public IP address. I checked the inbound rules in AWS and updated the SSH source to My IP. After saving the changes, I was able to connect to the server again.

I also initially ran the Apache status command in the wrong Ubuntu terminal. I learned that my local Ubuntu virtual machine and my AWS EC2 Ubuntu server were two separate environments. Since Apache had been installed on AWS, I needed to run the service commands inside the AWS server rather than my local virtual machine.

Overall, this practical activity helped me understand how Linux services are managed and monitored. I also learned that installing a service is only one part of server administration. It is equally important to check its status, validate its configuration and test whether it is accessible. These skills are useful for system administrators who need to maintain reliable and accessible servers.
