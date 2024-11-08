# Database Application (Part 1: LAMP Stack Configuration)

<div align="center">
  
 ![LAMP](https://imgur.com/wyxL02M.jpg) 
 
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
  - Begin by installing Apache on the Linux virtual machine deployed in VMware.
  - During the installation, we performed status checks to ensure proper configuration.

![install](https://imgur.com/jBQejrd.jpg)

![bad scripting](https://imgur.com/LBc9PUh.jpg) 

![back on track](https://imgur.com/4Bh8LdG.jpg)

2. Firewall Configuration:
  - Confirm that firewall services are available on ports 80 (HTTP) and 443 (HTTPS).
  - Use the following commands:

#
    firewall-cmd --permanent --add-service=http
    firewall-cmd --permanent --add-service=https
# 

## PHP and Dependencies Installation

1. EPEL and REMI Repositories:
   - Add the EPEL repository to the system.
   - Configure the REMI repository to access additional PHP packages.

![install epel](https://imgur.com/vXBZtD3.jpg) 

![config remi](https://imgur.com/JZ4vhgO.jpg) 

![remi enabled](https://imgur.com/zco7Ink.jpg) 

2. PHP Installation:
   - Install PHP using the appropriate package manager.
   - Verify that PHP is correctly installed and configured.

![php install](https://imgur.com/YNGoilw.jpg) 

3. PHP Extensions:
   - Install necessary PHP extensions.
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

![mariadb user setup/enable mysql](https://imgur.com/pxHT5iG.jpg) 

## phpMyAdmin Configuration
In the final installation step, we’ll explore the installation and configuration of phpMyAdmin—an essential administration tool for managing MySQL and MariaDB databases. phpMyAdmin provides a convenient web-based interface, allowing access to perform various database-related tasks.

1. Installing phpMyAdmin
   - Begin by installing phpMyAdmin on the server.
   - Verify that phpMyAdmin is correctly installed.

![phpmyadmin interface install](https://imgur.com/jCBMu0l.jpg) 

![config phpmyadmin](https://imgur.com/yHgH8GP.jpg) 

2. Configuring phpMyAdmin
   - Access the phpMyAdmin configuration file `/etc/phpMyAdmin/config.inc.php`).
   - Modify the configuration settings:
       - Grant Access: By default, phpMyAdmin allows access only from the localhost. We added a granted access to all hosts line for easier login.
       
![open phpmyadmin](https://imgur.com/YifEubJ.jpg) 

![open phpmyadmin2](https://imgur.com/aBWX388.jpg) 

3. Restarting Services
   - After making changes, restart the Apache service (`httpd.service`) to apply the configuration.

![open phpmyadmin3](https://imgur.com/ojQllTe.jpg) 

4. Initial Login
  - Access phpMyAdmin via web browser using the server’s IP address or domain name.
  - After encountering issues at login (“root login failure”), we troubleshooted by checking the configuration and user credentials.

![ip phpmyadmin](https://imgur.com/EJLmQpy.jpg) 

![http sever test](https://imgur.com/OPmEvyy.jpg) 

![phpmyadmin login](https://imgur.com/a5pimMP.jpg) 

![root login failure](https://imgur.com/gWZjdta.jpg) 

5. Temporary Password Setup
   - We opened the configuration file for phpMyAdmin 
   - To simplify initial access, we allowed login without a password (for the first sign-in).
   - We will change the password promptly after successful login.

![allownopw auth](https://imgur.com/yaxRtLy.jpg) 

![allownopw auth2](https://imgur.com/HSGIasf.jpg) 

6. Successful Database Login
   - Once configured, we should be able to log in successfully to phpMyAdmin.

![login success](https://imgur.com/fwrgRYW.jpg) 

## Conclusion
In Part 1 of this project, we successfully installed and configured the LAMP stack (**Linux**, **Apache**, **MySQL** and **PHP**). In Part 2 linked [here](https://github.com/jasminemathieu/Azure-SOC), we explore the interface and functionality of the phpMyAdmin database application.
