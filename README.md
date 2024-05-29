# Database Application (Part 1: LAMP Stack Configuration)

<div align="center">
  
 ![LAMP](https://imgur.com/LrpKNa7.jpg) 
 
</div>

## Introduction

This project covers the installation and configuration of a LAMP stack collection process. This LAMP stack is comprised of four programs - Linux, Apache, MySQL and PHP, used to create and deploy a functional database application. 

### Components used to complete this project:

- Linux
- Apache
- MySQL
- PHP
- VMware
- phpMyAdmin

## Apache Web Server Installation

Using a Linux virtual machine deployed on VMware, we begin this project with the installation of Apache. During this process I performed status checks to ensure proper configuration and started the Apache program. I mistakenly scripted the code as reflected in the 2nd image below and got back on track in the 3rd image.

![install](https://imgur.com/jBQejrd.jpg)

![bad scripting](https://imgur.com/LBc9PUh.jpg) 

![back on track](https://imgur.com/4Bh8LdG.jpg)

After Apache was successfully installed and turned on, I ensured firewall services on ports 80 and 443 were available by running the following commands:

`firewall-cmd --permanent --add-service=http` <br/>

`firewall-cmd --permanent --add-service=https`

## PHP and Dependencies Installation

I also restarted the firewalld.service after the ports were confirmed to be enabled. I started the PHP installation section of the process with adding the EPEL repository on the system, followed by REMI. I completed this step of the process with the PHP installation as displayed in the next 5 images.
![install epel](https://imgur.com/vXBZtD3.jpg) 

![config remi](https://imgur.com/JZ4vhgO.jpg) 

![remi enabled](https://imgur.com/zco7Ink.jpg) 

![php install](https://imgur.com/YNGoilw.jpg) 

![php extension install](https://imgur.com/1WU2rba.jpg) 

## MariaDB / MySQL Installation 

I installed php-mysql as displayed below and the supported fork of the MySQL, MariaDB to ensure access to MySQL’s data and table definition files and also identical client protocols, client APIs, ports, and sockets.

![install php mysql](https://imgur.com/J31VDcT.jpg) 

![install mariadb server](https://imgur.com/H09pOrL.jpg) 

![mariadb install complete](https://imgur.com/IbsfzN3.jpg) 

I ran a status check on Mariadb to confirm proper configuration and enabled the service.

![mariadb status check](https://imgur.com/eLXry5H.jpg) 

![open mariadb](https://imgur.com/1Jat4nX.jpg) 

I then started a secure installation of MySQL as reflected below.

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
