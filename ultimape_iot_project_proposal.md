#Nicholas Perry ([@ultimape](https://twitter.com/ultimape))'s Project Proposal:

###To create a proof-of-concept Internet of Things (IoT) network showcasing Eris Industries' systems. 

The main goal of this project is to create a simple monitoring/control website running on top of the Eris's Decerver that is able to interact with these devices. Eris's blockchain tech will further be used to manage the exchange (transaction) of messages between various sensor, displays, and actuators and allow for a decentralized way to manage a large and distributed 'Internet of Things'.

The project is a security minded modernization of my team's senior project 'smartHAuS' originating out of my degree work at Vermont Technical College. I will be taking heavy influence from a subsiquent project I was developing at Praetor Labs internally known as [Shardonnay](https://workflowy.com/s/493ab350-f171-d9c0-6ef1-f50c68ca65a6) in wich a distributed resource model was our primary goal. We were using [a cluster of ShuttlePCs](http://imgur.com/u31YJHO) to simulate embedded systems.

The project would leverage Eris' smart contracts to govern five key areas:

 - Ownership of a device may be exchanged between users
 - Assignment of access rights to various components on a device (read, write, modify-permissions, etc.)
 - Configuration of device-to-device transactions
 - Management of device meta-data (e.g. hard-coding location data or linking up a GPS subsystem)
 - A system to log/broker data in bulk to 3rd party networks ("peering") optionally paying for data via a bitcoin oracle.

###Current Direction

My plan is to target ubuntu-core (and debian) running on small number of Beaglebone Black and/or Raspberry Pi devices - as well as mocks running on VMs and (time permitting) integration with less powerful Arduino compatible devices. 

To simplify matters, user accounts and access rights would be modeled after Unix style permission systems & linked to the OS's filesystem. An agent service with SUDO permissions would be used to modify the filesystem permissions in response to changes announced within the blockchain, and a basic federated login system will be used to bootstrap account surrogates. Access to components would be created through a named pipe (or similar mechanism) to allow for OS enforcement. 

Device to device communication and data encryption - while interesting - are necessarily beyond the scope of this project, however an effort will be made to ensure it is solution agnostic.

I would be doing regular writeups on my progress with the goal of helping others to follow a similar journey. I am willing to do online talks and other promotional work as needed.

###Motivation

My motivations for a lot of what I do typically involve 3 key things:
 - My Mother: I want to help my disabled mother to be able to manage parts of her home from her bed.
 - Myself: I'm forgetful and want my house to help me do things. 
 - Mars: A robust distributed swarm of automated factories & farms on mars sounds like a cool thing to do.

I'm a big fan of OpenData initiatives and believe strongly in Free Open Source Software, Creative Commons, and Radical Transparency.  All this data we are generating should be given a chance to be free if people want it to be. I not see IoT (and by extension, the Quantified Self movement) getting big unless we conquer security, privacy, and ease of use concerns. I see Eris Industries' work being a key component of this vision. 

Or to put it simply: I hate the thought of a vendor owning my data, or the government knowing when I poop.

My wish is to inspire like-minded Makers (& Marmots) to get onboard with IoT and blockchain technology. I'd like to see work toward a system that makes it simple to get a device hooked up and start sharing in a secure way. 

Why am I applying as an internship? 
TL;DR: I have no idea what I'm doing.

###Simlar Projects

For similar projects in this space, refer to:

 - [@IBMIBV's ADEPT protocol](http://www.coindesk.com/ibm-reveals-proof-concept-blockchain-powered-internet-things/) - a yet to be finalized protocol proposal discussing a number of concerns. 
  - See a [demo at CES 2015](https://www.theprotocol.tv/adept-demo-ibm-samsung/).

 - [@Startstarad's TilePay ](https://twitter.com/Startstarad/status/578425604753747968) a managment ĐApp.
   - focusing on monetization via what appears to be a coloured coin.
   - Seems to be aiming for the creation of a marketplace.
