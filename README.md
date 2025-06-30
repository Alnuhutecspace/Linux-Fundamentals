# Linux-Fundamentals

## Introduction to Linux 

In the dynmaic landlandscape of mastering technology the fundamentals is essential for anybody aspiring to excel in the such as DevOps, Cloud Computing, Software Development, Cybersecurity, Data Analysis/Science, AI, and QA Testing. This project is designed to equip you with a solid foundation in Linux.Understanding the tech from the basics lays the groundwork for success in various tech-centrics careeres. 

## What is Linux? 

Linux is a free and open-source operating system (OS) that controls computer hardware and provides services for running software applications. It is based on the Unix operating system and is known for its stability, security, and flexibility. 

## Technical Definition 

At its core, Linux refers to the Linux kernel, the low-level software that manages hardware resources (CPU, memory, devices). Most people use "Linux" to mean a complete Linux-based operating system, which includes the kernel, system utilities, libraries, and user applications.

## Key Characteristics 

- Open Source: Anyone can view, modify, and distribute the code.

- Multiuser: Multiple users can use the system simultaneously without interfering with each other.

- Multitasking: Can run several programs at the same time.

- Portable: Runs on many types of hardware, from phones to supercomputers.

- Secure: Strong permissions system and frequent updates. 

## Linux vs Other Operating Systems

| Features | Linux | Windows | macOS |
| ----------- | ----------- | ----------- | ----------- |
| License | Open Source (GPL) | Proprietary | Proprietary |
| Cost| Free | Paid (usually) | Paid (bundled) |
| Customization | Very high | Low | Low |
| Common Use | Servers, Dev tools | Home/Office PCs | Apple Hardware |

## Common Linux Uses 

1. Web Servers (Apache, Nginx) 

2. Development Environments (especially for programming)

3. Embedded Systems (routers, TVs)

4. Supercomputing

5. Cybersecurity & Hacking (Kali Linux)

## Linux Distributions 

A Linux distribution is a collection of (usually open source) software on top of a Linux kernel. A distribution (or often refers to as **'distros'**) can bundle server software, system management tools, documentation and many desktop applications in a central secure software repository. A distro aims to provide a common look and feel, secure and easy software management and often a specific operational purpose. They offer different configurations, desktop environments, package managers, and software repositories, and then they are branded. Some of the linux distributions are; 

**Ubuntu**: Ubuntu is one of the most popular Linux distributions (distros). It's known for being user-friendly, free, and well-supported. Ubuntu is developed and maintained by a company called Canonical Ltd., and it's often the first Linux experience for new users, as well as for everyday desktop computing. Ubuntu has server edition for web hosting and cloud deployments. 

![Ubuntu Logo](./img/01.%20Ubuntu.png) 

**CentOS**: CentOS (short for Community ENTerprise Operating System) is a free and open-source Linux distribution based on Red Hat Enterprise Linux (RHEL). It's designed for enterprise environments, offering the same level of stability which is another distro itself, but requires paiide license. System administrators often choose CentOS because it's free reliable and robust. 

![CentOS](./img/02.%20CentOS.png) 

**Debian**: Debian is also known for its commitment to free and open-source software principles. Make Linux available for free, provides a wide range of software packages and supports multiple hardware architectures. 

![Debian](./img/04%20Debian.png) 

**Fedora**: Fedora is a cutting-edge distribution that focuses on integrating the latest software and technologies. It's a great choice for those who want to experiment with new features and applications. Fedora also serves as a testing ground for Red Hat's Enterprise Linux products. 

![Fedora](./img/03.%20Fedora.png) 


## Installation and Initial Setup 

In this section, we will create a server in the cloud, and gain access to it from our local environment. When we say "Local environment" we are referring to our laptop or the desktop PC we are using to work or learn. Which would have either Windows, or Mac operating system in most cases. Then you will connect to that server in the cloud, remotely staright from laptop. 

The setup will look like this 

![Server Connection](./img/05.%20Server%20Connection.png)  

Using [**AWS**](https://aws.amazon.com/), a public cloud provider to create the server in the cloud. AWS can provide us with a free virtual server called EC2 [Elastic Cloud Compute](https://aws.amazon.com/ec2/features/) 

**Let Us Create EC2 Instance. i.e a Linux Server** 

Watch the video below to get yourself setup. 

- [AWS account Setup and Provisioning an Ubuntu Server](https://youtu.be/xxKuB9kJoYM?si=lygzmDmttklV5-7l) 

- [Connecting to Your EC2 Instance](https://youtu.be/TxT6PNJts-s?si=THJvvZgLHBCr2XAG) 

Or follow the guideline below. 

**i. Register a new AWS account following** [this instruction](http://repost.aws/knowledge-center/create-and-activate-aws-account) 

- ii. Sign in to your AWS account 

![Conssole Home](./img/06.%20Console%20Home.png)

- iii. On the top left select services and search for Elastic Cloud Compute (EC2) 

![Search for EC2](./img/07.%20Search%20for%20EC2.png) 

- iv. From the menu on the left side, select instatnces. 

- v. Select launch instance on the top right side. 

![Locate and Launch Instance](./img/08.%20Locate%20and%20Launch.png)

- vi. Follow the image below to finish launching an instance. 

![Instance Success](./img/09.Instance%20Success.png)

## Connecting to the Server 

Now it's to get onto the server you have just created in the cloud you will need a number of things setup depending on your operating system. 

1. **A client tool**: A client tool, is a program on your computer that lets you communicate and give commands to a remote server. Imagine it as a doorway on your laptop that allows you to speak to a far-off computer as if it were right in front of you. By typing commands to terminal, you can ask the remote server to perform tasks, retrieve data, or even run programs, all without being physically present near the server. This is especially useful for managing websites, running software, or accessing files, from anywhere in the world, just by using simple text commands. 

2. **A secure protocol**: A secure protocol is like a protected path over the internet that ensures the information you send from your computer to a remote server is safe from prying eyes. Imagine sending a secret letter through a series of locked armored vehicles instead of a regular open road; that's what a secure protocol does for your data. It encrypts, or scrambles your information so that only intended recipient, the remote server can understand it. The popular protocol for this purpose is called **SSH (Secure Shell)**

## Client tools to install 

If you are on windows, you will need to have tools such as [MobaXterm](https://mobaxterm.mobatek.net/) installed. There are many other options such as: 

- [PuTTY](https://www.putty.org/) 

- [GitBash](https://git-scm.com/downloads) whichis available by default when you install Git on Windows. 

- Powershell - This is available by default on every Windows computer remotely, it is more optimised for Microsoft Windows. 

For simplicity, focus only on **MobaXterm** which is perfect for all you need throught this program. 

## Connection using SSH 

Now open the terminal, it is time to connect to remote serverthat was created.

Most client tools alraedy have SSh installed, so you literally don't have to do anything other than simply ytping the command 'ssh' on the terminal. 

1. Open the terminal 

2. Locate the "**pem key**" downloaded earlier. 

    1. Assuming it got downloaded in "Downloads" folder. 

    2. To navigate use Linux Command below. 

![Locate Folder](./img/10.%20Locate.Folder.png)

lets braekdown the command

- 'cd': Stand for "change directory" which is a command used to navigate between the folders in the terminal. 

- '~': Represent the home directory of the current user. It's a shortcut to refer to the user's primary directory without having to type out the full path. 

- '/Downloads': Specifies the Downloads folder, which is a common directory where files are saved when downloaded from the internet. 

3. Using the name for of the "**pem key**"
downloaded ealier for example 'ubuntu.pem', 'ls -l' command can be run and it will show the list of files in the "Downloads" folder, and 'ubuntu.pem should be listed in the folder. 

4. Extract the public IP address of the serveryou createdfrom AWS. 

![Locate Ip Adddress](./img/11.%20Public%20Ip%20Address.png) 

5. Connecting to the serverusing **SSH** simply run the comand below 

![Command to SSH](./img/12.%20Command%20to%20SSH.png)

Breaking down the command: 

    'ssh': This command to initiate on SSH connection. SSH is a protocol used to securely access and mange a remote system over an unsecured network (The Internet is an unsecured network). 

    '-i': "ubuntu.pem": The -i specifies the path to a private key file used for authentication. In this case. "ubuntu.pem" is a private key file. This file is essential for proving your identity to the server without needing a password. The .pem file is often used when connecting to server, for example those hosted on AWS (Amazon Web Service).

    'ubuntu@public_ip_address': This part specifies the user and the server you're trying to connect to. 'ubuntu' is the username on the remote serrver that you're logging in as , and 'public_ip_address' should be replaced withthe actual public IP address (or hostname) of the server you're trying to access. The  "@" symbol seperate the username from the server's address. 

Once the connection was successful established an output like this will be shown whhich prove that their is a connection to remote server. 

![Connect to SSH](./img/13.%20Connect%20to%20SSH.png) 


## Package Managers 

Most of the time when working on linux, there will be the need to install tools. Server are use to host websites, there has to be a tool that will help in the rendering of the web pages. A commonly used tool is called [Nginx](https://nginx.org/) 

Since the server are not regular computers where you can go to a browser to click and download, there is the need to have package managers that can help achieve this. 

Package manager in linux are not tools that automate the process of installing, updating, configuring and removing software packages on a linux server. They simplify the management of software by handling dependencies, versioning and installation procedures. These are several package managers used in various Linux distributions. 

## Commonly Used Package Managers APT (Advanced Package Tool): 
Used by Debian based distributions, such as Debian, Ubuntu, and derivatives. Commands include 'apt-get' and 'apt'. 

## Yum (Yellowing Updater Modified):
Originally used by Red Hat and CenOS. 'YUM' is now largely replaced by 'dnf' in modern Red Hat Based distributions It simplifies package management by resolving dependencies just like 'apt'. 

## DNF (Dandified YUM): 
Used in modern versions of Red-Hat-based distributions as a replacement for YUM. It provides improved performance and resolves some of the limitations of the older YUM tool. 


## Installing, Updating, and Removing Software 

Since we are on Ubuntu based server lets expplore how to install tools on a linux server. 

1. **Updating Package Lists** Before installing new software or updating existing packages. it's important to refresh the package lists. 

![Updating](./img/14.%20Updating.png) 

2. **Installing Software Packages** 

Lets try to install a command called 'tree' 

The 'tree' command is commonly used to visually see the file system structure on a linux server. So let's install it with the command below. 

Debian/Ubuntu 

![Install Tree](./img/15.%20Install%20Tree.png) 

If you were on other Linux distribution using 'yum',  the command would look like this. 

3. **Verifying Installed Packages** To confirm that the desired packagee or software has been successfully installed, simply run the 'tree' command and specify the path you wwant to see the tree structure. 

For Examplee; 

![Example](./img/16.%20Example.png)

Play around with this tree tool and specify different folders on the server. 

4. **Updating Installed Packages** keep your system up-to-date by updating installed packages. 

![Upgrade](./img/17.%20Upgrade.png)

5. **Removing Software Packages** To remove the 'tree' package we installed ealier run the command below 

![Removing](./img/18.%20Removing.png) 