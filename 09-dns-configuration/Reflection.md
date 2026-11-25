# Topic 9: Configuring DNS and Testing Domain Resolution

## DNS Configuration

In this activity, I worked with DuckDNS to configure a domain name for my AWS EC2 Ubuntu server. I used the domain `afiqahaws.duckdns.org` and configured its DNS record to point to my EC2 server's public IP address.

This allowed me to access my web server using a domain name instead of having to remember its numerical IP address.

## Testing Domain Resolution

After configuring the domain, I tested whether it could reach my Apache web server using:

`curl -I http://afiqahaws.duckdns.org`

The server returned `HTTP/1.1 200 OK`, confirming that the domain was reaching my Apache web server successfully.

## Learning Outcome

Through this activity, I learned how DNS connects domain names to IP addresses and makes web servers easier to access. I also understood the importance of checking DNS configuration when setting up websites and cloud services. This knowledge is useful for system administrators and network professionals who manage domains and server connectivity.
