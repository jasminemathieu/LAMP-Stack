# Database Application (Part 1: LAMP Stack Configuration)

<div align="center">
  
 ![LAMP](https://imgur.com/LrpKNa7.jpg) 
 
</div>

## Introduction

This project focuses on the installation and configuration of a LAMP stack—a combination of four essential components: **Linux**, **Apache**, **MySQL**, and **PHP**. The LAMP stack enables the creation and deployment of a functional database application. Below, I’ll break down each component and provide a clearer structure for your project.

## Components used to complete this project:

1. Linux
2. Apache
3. MySQL
4. PHP

Additional tools:
  - VMware
  - phpMyAdmin

## Apache Web Server Installation

1. Installation Process:
  - Begin by installing Apache on your Linux virtual machine deployed in VMware.
  - During the installation, perform status checks to ensure proper configuration.
  - If you encounter any issues (as seen in the “bad scripting” image), troubleshoot and correct them promptly.

![install](https://imgur.com/jBQejrd.jpg)

![bad scripting](https://imgur.com/LBc9PUh.jpg) 

![back on track](https://imgur.com/4Bh8LdG.jpg)

2. Firewall Configuration:
  - Confirm that firewall services are available on ports 80 (HTTP) and 443 (HTTPS).
  - Use the following commands:
After Apache was successfully installed and turned on, I ensured firewall services on ports 80 and 443 were available by running the following commands:
#
    firewall-cmd --permanent --add-service=http
    firewall-cmd --permanent --add-service=https
# 

## PHP and Dependencies Installation

1. EPEL and REMI Repositories:
   - Add the EPEL repository to your system.
   - Configure the REMI repository to access additional PHP packages.

![install epel](https://imgur.com/vXBZtD3.jpg) 

![config remi](https://imgur.com/JZ4vhgO.jpg) 

![remi enabled](https://imgur.com/zco7Ink.jpg) 

2. PHP Installation:
   - Install PHP using the appropriate package manager.
   - Verify that PHP is correctly installed and configured.

![php install](https://imgur.com/YNGoilw.jpg) 

3. PHP Extensions:
   - Install necessary PHP extensions for your project.
   - Ensure compatibility with the LAMP stack.

![php extension install](https://imgur.com/1WU2rba.jpg) 

## MariaDB / MySQL Installation 

1. php-mysql and MariaDB:
   - Install the php-mysql package to enable PHP’s interaction with MySQL.
   - Choose MariaDB as the MySQL fork for compatibility.

![install php mysql](https://imgur.com/J31VDcT.jpg) 

![install mariadb server](https://imgur.com/H09pOrL.jpg) 

![mariadb install complete](https://imgur.com/IbsfzN3.jpg) 

2. MariaDB Configuration:
   - Confirm proper configuration by checking the status of MariaDB.
   - Enable the MariaDB service.

![mariadb status check](https://imgur.com/eLXry5H.jpg) 

![open mariadb](https://imgur.com/1Jat4nX.jpg) 

3. Secure MySQL Installation:
   - Run a secure installation for MySQL.
   - Set up user accounts and access privileges.

![maria enabled](https://imgur.com/iMre9vk.jpg) 

I completed the authorization portion of the install that I believe caused as issue we will see later in this project. 

![mariadb user setup/enable mysql](https://imgur.com/pxHT5iG.jpg) 

## phpMyAdmin Configuration
In the final installation step, phpMyAdmin was successfully added. This administration tool for MySQL and MariaDB will act as a portable web application for the database.

![phpmyadmin interface install](https://imgur.com/jCBMu0l.jpg) 

![config phpmyadmin](https://imgur.com/yHgH8GP.jpg) 

I configured the phpMyAdmin to grant access to all instead of only the local host for easier login.

![open phpmyadmin](https://imgur.com/YifEubJ.jpg) 

![open phpmyadmin2](https://imgur.com/aBWX388.jpg) 

I then restarted and checked the httpd.service 
![open phpmyadmin3](https://imgur.com/ojQllTe.jpg) 

After copying the IP address set for the phpMyAdmin account, it was confirmed to work as reflected in the second image below.

![ip phpmyadmin](https://imgur.com/EJLmQpy.jpg) 

![http sever test](https://imgur.com/OPmEvyy.jpg) 

On the phpMyAdmin login page I experienced complications when attempting to enter the account, as reflected in the error message in the second image. 

![phpmyadmin login](https://imgur.com/a5pimMP.jpg) 

![root login failure](https://imgur.com/gWZjdta.jpg) 

I opened the configuration file for phpMyAdmin and changed the password requirements to have the ability to enter the site without a password for my first initial sign in with the plan to change the password upon entry to the account.

![allownopw auth](https://imgur.com/yaxRtLy.jpg) 

![allownopw auth2](https://imgur.com/HSGIasf.jpg) 

## Successful MYSQL Database Login
I completed the installation and configuration process as reflected with a successful entry into the database application.

![login success](https://imgur.com/fwrgRYW.jpg) 

## Conclusion
In part 1 of this project, I was able to successfully install and configure a LAMP stack combination consisting of Linux, Apache, MySQL and PHP programs and dependencies. In part 2, linked [here](https://github.com/jasminemathieu/Azure-SOC), I was able to demonstrate the functionality of the phpMyAdmin database that was configured.

## fin
