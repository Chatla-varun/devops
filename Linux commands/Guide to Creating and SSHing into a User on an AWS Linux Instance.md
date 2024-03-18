### Creating User in Linux:
1. Open a terminal window.
2. Use the `adduser` command to create a new user:
   ```bash
   sudo adduser <username>
## Changing Password Authentication to Yes:
Edit the SSH server configuration file using a text editor like nano or vim:

 sudo nano /etc/ssh/sshd_config
Locate the line PasswordAuthentication and change its value to yes.

## Restarting the SSH Service:
After making changes to the SSH configuration, restart the SSH service:

sudo systemctl restart sshd

## Connecting to Linux Machine with Username and Password:
Open a terminal window on your local machine.
Use the ssh command to connect to your Linux machine using the username and public IP address:

ssh <username>@<public_ip_address>
