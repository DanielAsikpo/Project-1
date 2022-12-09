# LAMP STACK IMPLEMENTATION ON AWS

## STEP 1 — INSTALLING APACHE AND UPDATING THE FIREWALL
### Update the linux package repository with the command below
`sudo apt update`

![image](./Images/Sudo_apt_update.png)

### Run apache2 package installation

`sudo apt install apache2`
![Images](./Images/Sudo_apt_install_apache%202.png)

### Verify that apache2 is running as a service in our OS

`sudo systemctl status apache2`

![Images](./Images/status%20_apache.png)

### If it is green and running, you've done everything right
**Kudus to you! You have just launched your first Web Server in the Cloud!**

### Before you can receive any traffic on your Web Server, you need make sure your security group settings on AWS allows TCP port 80 traffic (HTTP).

### You can try to check if it is locally running on your Ubuntu terminal using the follwing commands

`curl http://localhost:80` **(Acccessing through DNS)**

`curl http://127.0.0.1:80` **(Accessing through the IP address)**

![Image](./Images/Local_host.png)

###  Next step to take is to test how your Apache HTTP server can respond to requests from the Internet.

### Open a web browser of your choice and try to access following url

`http://<Public-IP-Address>` **(Public Address example: 55.11.22.226)**

### Kindly check your AWS console to get your public IP address

### If you see the following page, your web server has been properly installed and is now accessible through your firewall.


![Image](./Images/Apache_default_page.png)















