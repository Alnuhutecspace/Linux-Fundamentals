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

![CentOS]() 

**Debian**: Debian is also known for its commitment to free and open-source software principles. Make Linux available for free, provides a wide range of software packages and supports multiple hardware architectures. 

![Debian]() 

**Fedora**: Fedora is a cutting-edge distribution that focuses on integrating the latest software and technologies. It's a great choice for those who want to experiment with new features and applications. Fedora also serves as a testing ground for Red Hat's Enterprise Linux products. 

![Fedora]()

## Installation and Initial Setup 

In this section, we will create a server in the cloud, and gain access to it from our local environment. When we say "Local environment" we are referring to our laptop or the desktop PC we are using to work or learn. Which would have either Windows, or Mac operating system in most cases. Then you will connect to that server in the cloud, remotely staright from laptop. 

The setup will look like this 

![]()  

Using [**AWS**](https://aws.amazon.com/), a public cloud provider to create the server in the cloud. AWS can provide us with a free virtual server called EC2 [Elastic Cloud Compute](https://aws.amazon.com/ec2/features/) 

**Let Us Create EC2 Instance. i.e a Linux Server** 

Watch the video below to get yourself setup. 

- [AWS account Setup and Provisioning an Ubuntu Server](https://youtu.be/xxKuB9kJoYM?si=lygzmDmttklV5-7l) 

- [Connecting to Your EC2 Instance](https://youtu.be/TxT6PNJts-s?si=THJvvZgLHBCr2XAG) 

Or follow the guideline below. 

**i. Register a new AWS account following** [this instruction](http://repost.aws/knowledge-center/create-and-activate-aws-account) 

- ii. Sign in to your AWS account 

- iii. On the top left select services and search for Elastic Cloud Compute (EC2)

- iv. From the menu on the left side, select instatnces. 

- v. Select launch instance on the top right side. 

- vi. Follow the image below to finish launching an instance. 


