# INFORMATION ASSURANCE - FINAL PROJECT
by **Group 1 - BSCS 3B**
- Jomar Damot
- Kenn Louise Comprado
- Aina Mae Dela Justa
- Jushua Jay Delos Santos

## STEP-BY-STEP DOCUMENTATION 



### 1. Install Headless Raspbian OS into Raspberry Pi. ###

 - Raspberry Pi Imager is the quick and easy way to install Raspberry Pi OS and other operating systems to a microSD card, ready to use with your Raspberry Pi.
 Here is the link for the [Raspberry Pi Imager](https://www.raspberrypi.com/software/)
 ![Screenshot 2023-12-07 145420](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/e2574685-2757-4d49-a721-188f7f518d8a)

 - Open Raspberry Pi Imager. Choose Raspberrry Pi Device, Operating System, and Storage.
 ![Screenshot 2023-12-07 135408](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/ca526d3e-fe83-4ab8-bef8-6a7b401f41e4)

 - Choose **_Raspberry Pi 3_** as device, **_Raspberry Pi OS (Legacy)_** as operating system, and our **_32GB SD Card_** as storage.
 ![Screenshot 2023-12-07 135512](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/9e5fe390-dc24-4570-9de6-0588a0fa450a)
 ![Screenshot 2023-12-07 135541](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/5d91f9da-4a42-40e0-a2b4-148fe5e9640d)
 ![Screenshot 2023-12-07 135558](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/95cc7542-6144-4873-b516-4fb3a3f675a0)

 -  Click **Next** after choosing the storage, device and os then click **Edit Settings** to customize the OS Settings.
 ![Screenshot 2023-12-07 135634](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/d99d262e-2f36-4056-9eb7-4661712a5f01)

 - In the OS Customization, we set the host, username, and password as **iloveyou**. We configure our wireless LAN available which is **CSPC BayanihanNet** and set the wireless LAN   country to **PH.** After it I enable SSH and use password authentication, then click **Save**.
 ![Screenshot 2023-12-07 135810](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/8f8dd69e-c5e5-44f0-a515-b23864ae8db8)

 - Click **Yes** to apply our customized settings.
   ![Screenshot 2023-12-07 140959](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/b1f04a91-fa82-44d9-ae70-e237221f1837)

 > [!WARNING]
 - A warning message will appear that all existing data on our SD card will be erased. Click **Yes** to continue
  ![Screenshot 2023-12-07 135833](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/5378f87f-03f9-45ab-a6c3-e25cba283b61)

 - OS writing on our SD card will then start

![Screenshot 2023-12-07 135844](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/c75ec2ca-df1e-4e13-9766-88eadc471491)

![Screenshot 2023-12-07 135942](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/e8c848b2-cafc-4923-a4c2-77301fdccd3a)

 - In this case when you see that it is verifying you can just cancel this and proceed to the next step
  
![Screenshot 2023-12-07 140853](https://github.com/kentzyyo/INFO-ASSURANCE/assets/61936205/9e465d13-36c9-4316-ba62-5fdd8aafb04c)

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
- Run RealVNC Viewer and enter the IP address in the search bar. If the screen of the Raspberry Pi appeared on RealVNC, it means that it already established connection and control on the Raspberry Pi. 
   ![13](https://github.com/Jommmmmmm/jo/blob/main/13.png)
