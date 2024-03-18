### Creating User in Linux:
1. Connect to the machine as a root user.
2. Use the `adduser` command to create a new user:
   ```bash
   sudo adduser <username>
## Changing Password Authentication to Yes:
3. Edit the SSH server configuration file using a text editor like nano or vim:

   ```bash
   sudo nano /etc/ssh/sshd_config
Locate the line PasswordAuthentication and change its value to yes:

## Restarting the SSH Service:
4. After making changes to the SSH configuration, restart the SSH service:
  
   ```bash
   sudo systemctl restart sshd
## Connecting to Linux Machine with Username and Password:
Open a terminal window on your local machine.
Use the ssh command to connect to your Linux machine using the username and public IP address:

    ```bash
    ssh <username>@<public_ip_address>
