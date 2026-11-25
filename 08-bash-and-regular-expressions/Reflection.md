# Topic 8: Bash Scripting and Regular Expressions

## Bash Scripting
In this activity, I practised writing and executing a basic Bash script in Ubuntu. I created a file named hello.sh using Nano and added the #!/bin/bash line to indicate that the script should be executed using Bash. I used the echo command to display messages in the terminal.

After saving the file, I used chmod +x hello.sh to give it executable permission. I then ran the script using ./hello.sh and confirmed that the messages were displayed correctly.


## Regular Expressions
I also practised using regular expressions with the grep command. I created a text file named contacts.txt containing sample eight-digit phone numbers.

I used the command grep -E '^[89][0-9]{7}$' contacts.txt to search for numbers that start with 8 or 9 and contain exactly eight digits. The command successfully displayed the matching numbers.## Screenshots
