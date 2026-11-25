# Topic 10: Obtaining and Managing Digital Certificates with Let's Encrypt

## SSL Certificate Installation

In this activity, I configured an SSL certificate for my Apache web server using Let's Encrypt. Before installing the certificate, I checked that Apache was running and tested my DuckDNS domain, `afiqahaws.duckdns.org`, using the `curl` command.

I also configured the AWS EC2 security group to allow HTTPS traffic through port 443. I then installed Certbot and its Apache plugin using:

`sudo apt install certbot python3-certbot-apache`

Next, I ran `sudo certbot --apache -d afiqahaws.duckdns.org` to request and install the SSL certificate. Certbot successfully obtained the certificate and configured Apache to use HTTPS.

## Testing and Learning Outcome

I verified the HTTPS connection using:

`curl -I https://afiqahaws.duckdns.org`

The server returned `HTTP/1.1 200 OK`, confirming that the website was accessible through HTTPS.

Through this activity, I learned how SSL certificates help secure communication between a web server and its visitors. I also learned how Certbot simplifies certificate installation and schedules automatic renewal. This is useful for system administrators because securing web services helps protect data exchanged between users and servers.
