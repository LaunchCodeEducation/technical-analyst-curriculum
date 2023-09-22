---
title: 7. Troubleshooting
weight: 107
---

## Existing documentation and knowledge systems
***
Many large and medium sized organizations that have been around for several years already have a large number of contributions from many different contractors and engineers. These existing documents, software and comments are part of the organization's knowledge management system or knowledge base. We can search these knowledge base systems to find answers to questions that we have or to troubleshoot an issue. Poor documentation leads to poor support and negatively impacts technical support. When we are new to our teams, we are not expected to know everything but we are expected to learn where and how to find the information we need. We should ask often for links to documentation that will provide more in depth learning of a given topic or subject. Once we have a fresh understanding and new perspective of the software product, we can ask questions using the referenced documentation links. If the documentation only lives in a single developer’s head, we should learn how it is done and document it and share it with the developer/engineer to ensure you've captured the steps properly. Then share it with the larger team.

**Pro tip:** Take note of the last updated date when reading documentation. We want to look for versions, last edited, last changed to ensure the documentation is still relevant. This tells us if the document is still changing but more importantly, if there is active participation with keeping the documentation updated.  

## What Are Standards and Policies

Standards are a uniformed way to create or build a system in software that everyone has to follow. They help us establish the normal way of performing a task. Polices are the special rules to follow that govern the task being performed in an organized and uniformed way. For example, when we write our names on an online employment application, we capitalize the first letters of our first and last name and we can use digital ink (soft copies). However, when we get hired, we use our signature on the legally binding documents in blue or black ink (also referred to as hard copies). The policy says all other documents signed in any other color are not to be reviewed or they are not considered completed. 

In software design, we need standards and policies to ensure we build the right system, the same way, every time. Without standards and policies every engineer could implement their own designs very differently leading to project delay and late project delivery. Part of troubleshooting requires understanding the application architecture, networking (aka communication) and object-oriented programming (OOP) concepts. Many software products today contain an OOP design implementation. We need to understand the fundamentals to better understand the problem. Object oriented programming is creating reusable software that can be implemented in other systems. 

Think of OOP it like home decor. Let’s say we designed a primary bedroom that had a water fountain, large floor carpet, ceiling fan, large windows and walk-in closet. Then we buy our second home but this time, we want the same room but different color carpet and no ceiling fan. In real life, we would have to move all of our things from the old room to the new one. In OOP we just instantiate the class (Room house2 = new Room()) and remove the methods for the ceiling fans and carpet. This is similar to copying and pasting all the items from house 1 primary bedroom to house 2 primary bedroom (minus the features we’d like to change) without the need to start from scratch with a new design. In object-oriented programming the Room object would be known as a class. We could take this example a step further and create every object in the room as a class/object itself, and give each object its own properties (colors, height, width etc.) but that is a bit more complicated to explain but is possible in this design concept. 

## Intro to Basic Networking

Networking is about connectivity from machine to machine in most instances. This could be computer to computer or laptop to Wireless Fidelity (WIFI) router. Recall in the section on “Effective Communication” Chapter where we talk about clear communication between people. Networking in social spaces or with computers is all about communication. The media we choose to communicate over (WIFI, ethernet, Bluetooth etc.) is just the medium to the other device on the network. A critical component of communication is device endpoints. If we know the device, we are connecting to we can create a proper connection. For example, inside Launch Code, our laptops can connect to the Launch Code sponsored WIFI. In order to connect to the router, we need the WIFI password. Once we have the password, we will be routed to the modem that is connected to our Internet Service Provider (ISP), then to the site we requested. What happens if we have a working password and we cannot get to the site we requested? This is where basic connectivity troubleshooting can help us diagnose the problem. We first need to understand the application architecture of the systems we’re using then we can begin troubleshooting. 

## Application Architecture

This document describes the behaviors and interactions of the applications we use in business. Physical and logical diagrams are used to help design the applications. The physical and logical diagrams are also used as reference points when troubleshooting common problems with the network. These diagrams are a great starting point for us to get familiar with the applications we support. 

**Pro Tip:** Always ask for a logical or physical application diagram when working a technical support role.   

The Open Systems Interconnection (OSI) Model is a conceptual framework that _standardizes_ the functions of networking or telecommunications into seven distinct layers.

1. Physical ( Layer 1) 
2. Data Link ( Layer 2)
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

**FTP (File Transfer Protocol) **, is used for transferring files between computers on a network. It allows users to upload and download files from remote servers.

**Firewalls**, a network security software that monitors incoming and outgoing network traffic based on security rules. They establish barriers between trusted networks and untrusted networks.


