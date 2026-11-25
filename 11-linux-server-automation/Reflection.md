# Topic 11: Scripting Linux Server Functions for Automation

## Server Automation Script

In this activity, I created a Bash script named `server-check.sh` on my AWS EC2 Ubuntu server. The purpose of the script was to automate basic server health checks instead of having to enter each command separately.

The script displayed the current date and time using `date`, checked disk usage using `df -h /`, displayed memory information using `free -h`, and checked whether Apache was running using `systemctl is-active apache2`.

After creating the script using Nano, I gave it executable permission with:

`chmod +x server-check.sh`

I then executed it using:

`./server-check.sh`

The script ran successfully and displayed the server information. Apache returned an `active` status, confirming that the web server was running.

## Learning Outcome

Through this activity, I learned how Bash scripting can automate repetitive Linux server administration tasks. Combining several commands into one script makes it easier to perform regular checks and monitor important server information. This is useful in system administration and DevOps because automation can reduce manual work and make server monitoring more efficient.
