# Database Application (Part 1: LAMP Stack Configuration)

<div align="center">
  <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" height="120" alt="linux logo"  />
  <img width="36" />
  <img src="https://seeklogo.com/images/A/apache-logo-89257496F9-seeklogo.com.png" height="120" alt="apache logo"  />
  <img width="36" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mysql/mysql-original.svg" height="120" alt="mysql logo"  />
  <img width="36" />
  <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/27/PHP-logo.svg/2560px-PHP-logo.svg.png" height="110" alt="PHP logo"  />
  <img width="30" />
</div>

## Introduction

This project covers the installation and configuration process of LAMP stack collection process. This LAMP stack is comprised of four programs - Linux, Apache, MySQL and PHP, used to create and deploy a functional database application. 

### Components used to complete this project:

- Linux
- Apache
- MySQL
- PHP
- VMware
- phpMyAdmin

## Apache Web Server Installation

We begin this project with the installation of a Apache. During this process I performed status checks and started the program. I mistakenly scripted the code as reflected in the 2nd image below and got back on track in the 3rd image.

![install](https://imgur.com/jBQejrd.jpg)

![bad scripting](https://imgur.com/LBc9PUh.jpg) 

![back on track](https://imgur.com/4Bh8LdG.jpg)

After a successful install and start for Apache, I managed the firewall on ports 80 and 443.
![firewall config](https://imgur.com/DpZ6Tx1.jpg) 

Following the firewall configuration, I started the PHP installation process, beginning with the configuration of EPEL repository on the system. I then configured REMI and completed this step of the process with PHP installation.
![install epel](https://imgur.com/vXBZtD3.jpg) 

![config remi](https://imgur.com/JZ4vhgO.jpg) 

![remi enabled](https://imgur.com/zco7Ink.jpg) 

![php install](https://imgur.com/YNGoilw.jpg) 

![php extension install](https://imgur.com/1WU2rba.jpg) 

## MariaDB Installaion

This portion of the project will cover the ...

![install php mysql](https://imgur.com/J31VDcT.jpg) 

The backup restore asset has been configured as displayed below....

![install mariadb server](https://imgur.com/H09pOrL.jpg) 

After unsuccessful attempts of accessing the virtual...

![mariadb install complete](https://imgur.com/IbsfzN3.jpg) 

I ran into complications when assigning a public...

![mariadb status check](https://imgur.com/eLXry5H.jpg) 

![open mariadb](https://imgur.com/1Jat4nX.jpg) 

From here I was able to configure a...

![maria enabled](https://imgur.com/iMre9vk.jpg) 

The IP address configuration was complete...
![mariadb user setup/enable mysql](https://imgur.com/pxHT5iG.jpg) 

## PHPMYADMIN Configuration
![phpmyadmin interface install](https://imgur.com/jCBMu0l.jpg) 

![config phpmyadmin](https://imgur.com/yHgH8GP.jpg) 

![open phpmyadmin](https://imgur.com/YifEubJ.jpg) 

![open phpmyadmin2](https://imgur.com/aBWX388.jpg) 

![open phpmyadmin3](https://imgur.com/ojQllTe.jpg) 

I used the IP address set for my phpmyadmin account. The IP address has been confirmed to work as reflected in the second image below.

![ip phpmyadmin](https://imgur.com/EJLmQpy.jpg) 

![http sever test](https://imgur.com/OPmEvyy.jpg) 

Moving on the phpmylogin page, I experienced some complications when trying to get into the account. As reflected in the error message in the second image, I opened the configuration file for phpmyadmin and changed the password requirements to have the ability to enter the site without a password for my first initial sign in with the plan to change the password once I'm in.

![phpmyadmin login](https://imgur.com/a5pimMP.jpg) 

![root login failure](https://imgur.com/gWZjdta.jpg) 

![allownopw auth](https://imgur.com/yaxRtLy.jpg) 

![allownopw auth2](https://imgur.com/HSGIasf.jpg) 

## Successful MYSQL Database Login
I was able to complete the installion and configuration process with a successful entry into the database application.

![login success](https://imgur.com/fwrgRYW.jpg) 

## Conclusion
In this project, I was able to successfully configure and complete a full cloud-native backup service and machine restore to 100% data availability in Azure. Both methods prove to be powerful on-premises data protection solutions, useful in events of service disruptions, accidental deletions or corruption of data. It's equally secure, scalable, and cost-effective as it is simple to architect, highly available, and resilient.

## fin
