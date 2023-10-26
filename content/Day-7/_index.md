---
title: 7. Troubleshooting
weight: 107
---

## Existing documentation and knowledge systems

Many large and medium-sized organizations, with years of history, have accumulated a wealth of contributions from various contractors and engineers. These contributions include existing documents, software, and comments, all integrated into the organization's knowledge management system or knowledge base. These knowledge base systems serve as valuable resources, allowing us to search for answers to our questions or troubleshoot issues.

Poor documentation can lead to inadequate support and have a detrimental effect on technical support. As newcomers to our teams, it's understood that we won't have all the answers from the get-go, but we are expected to learn where and how to access the necessary information. It's essential to frequently request links to documentation that offer in-depth insights into specific topics or subjects.

Once we've gained a solid understanding and a fresh perspective on the software product, we can ask questions using the provided documentation links. In cases where documentation resides solely in the mind of a single developer, it's crucial to learn the process, document it accurately, and share it with the developer or engineer to ensure the steps are correctly captured. Subsequently, share this documented knowledge with the larger team.

{{% notice green "Protip" "rocket" %}}
Take note of the last updated date when reading documentation. We want to look for versions, last edited, last changed to ensure the documentation is still relevant. This tells us if the document is still changing but more importantly, if there is active participation with keeping the documentation updated.  
{{% /notice %}}

## What Are Standards and Policies

Standards and policies play a vital role in software development, ensuring that systems are consistently created and that tasks are performed uniformly. Standards provide a structured way to build a system that everyone must adhere to, while policies are specific rules governing the organized and uniform execution of tasks.

For instance, consider the practice of signing one's name on an online employment application. Standards dictate that we capitalize the first letters of our first and last names, and we can use digital ink (soft copies). However, when it comes to legally binding documents upon being hired, policies require us to use our signature in blue or black ink (hard copies). Any other colors are not accepted or considered as completing the document.

In software design, standards and policies are essential to ensure that systems are constructed consistently and accurately. Without these guidelines, engineers might implement designs in vastly different ways, leading to project delays and late deliveries. Troubleshooting in the software field also necessitates a solid grasp of application architecture, networking (communication), and object-oriented programming (OOP) concepts. Many modern software products are built using an OOP design, making it crucial to understand the fundamentals for effective problem-solving.

To grasp the concept of object-oriented programming, consider it like home decor. Imagine designing a primary bedroom with specific features, and later, you want the same room but with a different color carpet and no ceiling fan. In real life, you'd need to move all your belongings from the old room to the new one. However, in OOP, you create an instance of the class (e.g., Room house2 = new Room()), remove the methods for the ceiling fan and carpet, and the new room is ready. This is akin to copying and pasting all the items from the first primary bedroom to the second, with the changes you desire, without starting from scratch with a new design.

In object-oriented programming, the Room object is known as a class, and you can take this concept further by creating each object in the room as a class with its unique properties (colors, height, width, etc.), although this is a more advanced aspect of the design concept.

## Intro to Basic Networking

Networking is primarily about establishing connectivity between devices. This connection could be between computers, laptops, or between a laptop and a Wireless Fidelity (WIFI) router. In the section on "Effective Communication," we discussed the importance of clear communication between people. Networking, whether in social spaces or with computers, revolves around communication. The choice of communication medium (such as WIFI, ethernet, Bluetooth, etc.) serves as the conduit to the other device on the network.

A crucial aspect of communication in networking is device endpoints. Knowing the specific device you are connecting to is essential for establishing a proper connection. For instance, within Launch Code, our laptops can connect to the Launch Code-sponsored WIFI. To connect to the router, we require the WIFI password. Once we have the password, we follow a path from the modem connected to our Internet Service Provider (ISP) to the site we wish to access.

However, what if we have a working password but still can't reach the desired site? This is where basic connectivity troubleshooting becomes valuable. First, we need to understand the application architecture of the systems we're using, and from there, we can begin the troubleshooting process.

## Application Architecture

This document describes the behaviors and interactions of the applications we use in business. Physical and logical diagrams are used to help design the applications. The physical and logical diagrams are also used as reference points when troubleshooting common problems with the network. These diagrams are a great starting point for us to get familiar with the applications we support. 

{{% notice green "Protip" "rocket" %}}
Always ask for a logical or physical application diagram when working a technical support role.   
The Open Systems Interconnection (OSI) Model is a conceptual framework that _standardizes_ the functions of networking or telecommunications into seven distinct layers.
{{% /notice %}}

1. Physical (Layer 1) 
2. Data Link (Layer 2)
3. Network (Layer 3) 
4. Transport (Layer 4) 
5. Session (Layer 5) 
6. Presentation (Layer 6)
7. Application (Layer 7)

**Physical-1** this is the lowest layer of the OSI Reference Model is layer 1, the physical layer; it is commonly abbreviated PHY. This layer is the only one where data is physically moved across the network interface. All other layers perform functions to create messages that implement various protocols, but these messages must all be transmitted down the protocol stack to the physical layer, and they are eventually sent out over the network. The physical layer technologies deal with the actual ones and zeros that are sent over the network.

**Data Link-2** is simply called the link layer, or abbreviated DLL. This layer is often conceptually divided into two sublayers called the logical link control (LLC) and media access control (MAC). This layer is where many wired and wireless local area networks (LAN) technologies primarily function. 

**Network-3** defines how internetworks (interconnected networks) function. This network layer is the lowest one in the OSI model that is concerned with actually getting data from one computer to another, even if it is on a remote network. In contrast, the data link layer only deals with devices that are local to each other via the LAN.

**Transport-4** the transport layer acts as a liaison between the abstract world of applications and the layers 1 to 3. layers 1 through 3 are concerned with the actual packaging, addressing, routing, and delivery of data to other machines. 

**Session-5** layer is responsible for addressing, packaging, and delivery of data. This layer is mainly concerned with software application issues and not with the details of network (the functions of layers 1-3)

**Presentation-6** this layer is charged with taking care of any issues that might arise when data sent from one system needs to be viewed (presented) in a different way by the receiving system. For example, Windows OS, MAC OS and Linux systems all have similar functionality but different file systems architecture. So data sent to each system will need to be translated to the specific machine instructions. 

**Application-7** It's important to understand that the OSI model application layer is not the same as an app or application. In the OSI model, this layer provides services for user applications to use. For example, when we use our web browser, that actual software is an application. It doesn't really reside at the application layer. It makes use of the services offered by a protocol that operates at the application layer, which is called the Hypertext Transfer Protocol (HTTP or HTTPS). 

Understanding the OSI model can help us reduce the number of hours we spend troubleshooting down from hours to minutes. Once we know how our application is communicating and what our application is communicating with, we can take the appropriate steps to resolve any issues we find within the application. Knowing where to look is more important that knowing all the steps needed to resolve the problem. After all, the steps are dynamic. 

## Network Terms 

Other network terms jargon you should be familiar with are listed below. This is intended to be a reference and not an exhaustive list. We expect that you will take this list and build upon it. Below are just a few examples of the many protocols that make up the TCP/IP suite. These protocols enable a seamless communication and data exchange that we experience on the internet and local networks.

**TCP/IP**, Transmission Control Protocol/Internet Protocol a suite of networking protocols that form the basis for communication on the internet and private networks. It provides a set of rules and conventions for how data should be sent, received, and routed between devices on a network. 

**Host / Hostname**, is a reference to the machine we are logged into. The Hostname is the name of the server in most cases.

**IP (Internet Protocol)**, is responsible for addressing and routing packets of data so that they can travel across networks and arrive at the correct destination. It assigns unique IP addresses to devices and handles the logical addressing of data packets.

**TCP (Transmission Control Protocol)**, is a reliable, connection-oriented protocol that provides error checking, sequencing, and flow control for data transmission. It ensures that data sent from one device arrives intact and in the correct order at the receiving device.

**UDP (User Datagram Protocol)**, is a simpler, connectionless protocol that does not provide the same level of error checking and sequencing as TCP. It is often used for applications where speed and efficiency are more important than data reliability, such as streaming media or online gaming.

**ICMP (Internet Control Message Protocol)**, is used for sending error messages and operational information about the network. It's often used by network devices to report errors, such as when a destination is unreachable.

**ARP (Address Resolution Protocol)**, is used to map IP addresses to physical MAC addresses on a local network. It helps devices find each other's physical addresses when communicating within the same subnet.

**DNS (Domain Name System)**, while not a core TCP/IP protocol, DNS is a critical component of internet communication. It translates human-readable domain names (like www.example.com) into IP addresses that computers can understand.

**HTTP (Hypertext Transfer Protocol)**, transmitting web pages and other resources over the internet. It defines how web browsers and servers communicate.

**SMTP (Simple Mail Transfer Protocol)**, is used for sending and receiving emails. It's responsible for transferring emails from the sender's email client to the recipient's email server.

**FTP (File Transfer Protocol)**, is used for transferring files between computers on a network. It allows users to upload and download files from remote servers.

**Firewalls**, a network security software that monitors incoming and outgoing network traffic based on security rules. They establish barriers between trusted networks and untrusted networks.


