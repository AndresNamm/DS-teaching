---
layout: default 
title: Indirext communication
---


# References

1. [Publish subsrcribe patters]https://docs.oracle.com/cd/B10501_01/appdev.920/a96590/adg15pub.htm
2. [Indirect communication slides ](https://www.kth.se/social/upload/504cf76ef27654461c000000/indirect%20communication.pdf)
3. [Indirect communication slides](https://www.ida.liu.se/~TDDD25/lectures/lect3.frm.pdf)

- Server sends information in a space and time unoupled manner. Only clients who have registered to the service get the message. 

# Space uncoupling 

+ The sender does not know, or need to 
know the receiver and vice versa
+ example - RSS 

# Time uncoupling 

+ Onedrive, Google docs, email


# Example systems of indirect communication

## Group communication  

Almost same as multicast but with more abstracted group management. 
Reliable dissemination of information to potentially large 
numbers of clients, including  financial industry, where  institutions require accurate and up- to-date access to a wide  variety of information sources

## Publish subsrcibe sytem 

Similiar to group communication, but now there exists a publish responsibility for certain entities and listening role for the clients, The clients can in short register for certain services that the server offers. Clients get only what they have subscribed themselves for. 
