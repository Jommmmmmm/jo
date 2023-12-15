# INFORMATION ASSURANCE - FINAL PROJECT
by **Group 10 - BSCS 3B**
- Jomar Damot
- Kenn Louise Comprado
- Aina Mae Dela Justa
- Jushua Jay Delos Santos

## STEP-BY-STEP DOCUMENTATION ON RASPBERRY PI OS



### 1. Install Raspbian OS into Raspberry Pi. ###

 - To install rasberry pi os we need to use rasPberry pi imager
 Here is the link for the rasberry pi imager [Raspberry Pi Imager](https://www.raspberrypi.com/software/)
 ![14](https://github.com/Jommmmmmm/jo/blob/main/14.png)

 - Open Raspberry Pi Imager. Choose Raspberrry Pi Device, Operating System, and Storage.
 ![15](https://github.com/Jommmmmmm/jo/blob/main/15.png)

 - Choose **_Raspberry Pi 3_** as device, **_Raspberry Pi OS (Legacy)_** as operating system, and our **_8GB SD Card_** as storage.
 ![16](https://github.com/Jommmmmmm/jo/blob/main/16.png)
 ![17](https://github.com/Jommmmmmm/jo/blob/main/17.png)

 -  Click **Next** after choosing the storage, device and os then click **Edit Settings** to customize the OS Settings.
 ![18](https://github.com/Jommmmmmm/jo/blob/main/18.png)

 - In the OS Customization, we set the host, username, and password as **iloveyou**. We configure our wireless LAN available which is **CSPC BayanihanNet** and set the wireless LAN   country to **PH.** After it I enable SSH and use password authentication, then click **Save**.
 ![19](https://github.com/Jommmmmmm/jo/blob/main/19.png)

 - Click **Yes** to apply settings.
   ![20](https://github.com/Jommmmmmm/jo/blob/main/20.png)

 > [!WARNING]
 - A warning message will appear that all existing data on our SD card will be erased. Click **Yes** to continue
  ![21](https://github.com/Jommmmmmm/jo/blob/main/21.png)

 - Then it wil start the OS writing on our SD card 

![22](https://github.com/Jommmmmmm/jo/blob/main/22.png)

![23](https://github.com/Jommmmmmm/jo/blob/main/23.png)

 - In this case when you see that it is verifying you can just cancel this and proceed to the next step
  
![24](https://github.com/Jommmmmmm/jo/blob/main/24.png)

### 2. Connect to Raspberry Pi via SSH using command prompt###
 - In the command prompt, type SSH to access the network protocol. Then type the following command:
   - ssh username@hostname
   - sudo apt update
   - sudo apt upgrade
     
 ![1](https://github.com/Jommmmmmm/jo/blob/main/1.png)

### 3. Install LAMP Stack
 - Install all the necessary requirements
 - To install the stack, type the following commands on our command prompt connected to Raspberry Pia via SSH.
   + **_sudo apt install apache2_**
   + **_sudo apt install mariadb-server_**
   + **_sudo mysql_secure_installation_**
   + **_sudo apt install php libapache2-mod-php php-mysql_**
   + **_sudo apt-get install php_**
   + **_sudo apt install phpmyadmin_**
     ![2](https://github.com/Jommmmmmm/jo/blob/main/2.png)
     ![3](https://github.com/Jommmmmmm/jo/blob/main/3.png)
     ![4](https://github.com/Jommmmmmm/jo/blob/main/4.png)
     ![5](https://github.com/Jommmmmmm/jo/blob/main/5.png)
     ![6](https://github.com/Jommmmmmm/jo/blob/main/6.png)
     

### 4. Connect to Raspberry Pi via VNC
 - Install RealVNC® Viewer by clicking this link [link](https://www.realvnc.com/en/connect/download/viewer/)
 - Before opening VNC on our PC, access first the Raspberry Pi Configuration Tool to enable VNC on the OS via the **_sudo raspi-config_** command.
 - Using the arrows, navigate to **'Interfacing Options'** > **'VNC'**, then choose **'Yes'** and select **'OK'** 
    ![8](https://github.com/Jommmmmmm/jo/blob/main/8.png)
    ![9](https://github.com/Jommmmmmm/jo/blob/main/9.png)
    ![10](https://github.com/Jommmmmmm/jo/blob/main/10.png)
    ![11](https://github.com/Jommmmmmm/jo/blob/main/11.png)
- The lastly we can Run RealVNC Viewer and enter the IP address taht we use earlier. If the screen of the Raspberry Pi appeared on RealVNC, it means that it already established connection and control on the Raspberry Pi. 
   ![13](https://github.com/Jommmmmmm/jo/blob/main/13.png)
