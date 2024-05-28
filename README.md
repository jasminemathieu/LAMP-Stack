# LAMP Stack Configuration

![Lamp image](https://imgur.com/Ylqw4gU.jpg)

## Introduction

This project covers the installation and configuration process of LAMP stack collection process. This LAMP stack is comprised of four programs - Linux, Apache, MySQL and PHP, used to create and deploy a functionmal database application. 

### Components used to complete this project:

- Linux Centos Stream 9
- Apache
- MySQL
- PHP
- VMware

## Apache Web Server Installation

We begin this project with the installation of a Apache. During this process I performed status checks and started the program. I mistakenly scripted the code as reflected in the 2nd image below and got back on track in the 3rd image.

![install](https://imgur.com/jBQejrd.jpg)

![bad scripting](https://imgur.com/LBc9PUh.jpg) 

![back on track](https://imgur.com/4Bh8LdG.jpg)

After a successful install and start for Apache, I managed the firewall on ports 80 and 443.
![firewall config](https://imgur.com/DpZ6Tx1.jpg) 

Following the firewall configuration, I started the PHP installation process, beginning with the configuration of EPEL repository on the system. I then configured REMI and completed this step of the process with PHP installation.
![delete test items2](https://imgur.com/vXBZtD3.jpg) 

On the virtual machine, the executable was ran in PowerShell ...
![powershell process](https://imgur.com/JZ4vhgO.jpg) 

![powershell complete](https://imgur.com/zco7Ink.jpg) 

## Backup Service - File Recovery Successfully Completed

The backup can be found in the D drive where we can see ...

![d drive](https://imgur.com/YNGoilw.jpg) 

![unmounted2](https://imgur.com/1WU2rba.jpg) 

# Part 2 - Restore VM

## Backup via Restore 

This portion of the project will cover the ...

![restore vm start](https://imgur.com/J31VDcT.jpg) 

The backup restore asset has been configured as displayed below....

![config complete](https://imgur.com/H09pOrL.jpg) 

After unsuccessful attempts of accessing the virtual...

![recoveredvm no ip2](https://imgur.com/IbsfzN3.jpg) 

I ran into complications when assigning a public...

![ip issues](https://imgur.com/eLXry5H.jpg) 

![take2](https://imgur.com/1Jat4nX.jpg) 

From here I was able to configure a...

![ip config2](https://imgur.com/iMre9vk.jpg) 

The IP address configuration was complete...
![ip complete](https://imgur.com/pxHT5iG.jpg) 

I then created inbound rules to ...

![RDP config2](https://imgur.com/jCBMu0l.jpg) 

![RDP confirmed](https://imgur.com/yHgH8GP.jpg) 

## Successful Restore Confirmation
I was able to remote into the machine and confirm the restore machine duplication was successful.

![confirm restore](https://imgur.com/YifEubJ.jpg) 

I ran into complications when assigning a public...

![ip issues](https://imgur.com/aBWX388.jpg) 

![take2](https://imgur.com/ojQllTe.jpg) 

From here I was able to configure a...

![ip config2](https://imgur.com/EJLmQpy.jpg) 

The IP address configuration was complete...
![ip complete](https://imgur.com/OPmEvyy.jpg) 

I then created inbound rules to ...

![RDP config2](https://imgur.com/a5pimMP.jpg) 

![RDP confirmed](https://imgur.com/CDaO1A6.jpg) 

## Successful Restore Confirmation
I was able to remote into the machine and confirm the restore machine duplication was successful.

![confirm restore](https://imgur.com/gWZjdta.jpg) 

I ran into complications when assigning a public...

![ip issues](https://imgur.com/yaxRtLy.jpg) 

![take2](https://imgur.com/HSGIasf.jpg) 

From here I was able to configure a...

![ip config2](https://imgur.com/fwrgRYW.jpg) 

The IP address configuration was complete...
![ip complete](https://imgur.com/SyKNHBB.jpg) 

I then created inbound rules to ...

![RDP config2](.jpg) 

![RDP confirmed](.jpg) 

## Successful Restore Confirmation
I was able to remote into the machine and confirm the restore machine duplication was successful.

![confirm restore](.jpg) 

I ran into complications when assigning a public...

![ip issues](.jpg) 

![take2](.jpg) 

From here I was able to configure a...

![ip config2](.jpg) 

The IP address configuration was complete...
![ip complete](.jpg) 

I then created inbound rules to ...

![RDP config2](.jpg) 

![RDP confirmed](.jpg) 

## Successful Restore Confirmation
I was able to remote into the machine and confirm the restore machine duplication was successful.

![confirm restore](.jpg) 

I ran into complications when assigning a public...

![ip issues](.jpg) 

![take2](.jpg) 

From here I was able to configure a...

![ip config2](.jpg) 

The IP address configuration was complete...
![ip complete](.jpg) 

I then created inbound rules to ...

![RDP config2](.jpg) 

![RDP confirmed](.jpg) 

## Conclusion
In this project, I was able to successfully configure and complete a full cloud-native backup service and machine restore to 100% data availability in Azure. Both methods prove to be powerful on-premises data protection solutions, useful in events of service disruptions, accidental deletions or corruption of data. It's equally secure, scalable, and cost-effective as it is simple to architect, highly available, and resilient.

## fin
