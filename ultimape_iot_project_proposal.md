#Nicholas Perry ([@ultimape](https://twitter.com/ultimape))'s Project Proposal:

###To create a proof-of-concept Internet of Things (IoT) network showcasing Eris Industries' systems. 

The main goal of this project is to create a simple monitoring/control website running on top of Eris's Decerver that is able to interact with IoT devices. Eris's blockchain tech will further be used to manage the exchange (transaction) of messages between various sensor, displays, and actuators and allow for a decentralized way to manage a large and distributed 'Internet of Things'.

The project is a security minded modernization of my senior project team's 'smartHAuS' originating out of my degree work at Vermont Technical College. I will also be taking heavy influence from a subsequent project I was developing at Praetor Labs internally known as [Shardonnay](https://workflowy.com/s/493ab350-f171-d9c0-6ef1-f50c68ca65a6) as it ended up having a distributed resource model as our primary goal. WHile were using [a cluster of ShuttlePCs](http://imgur.com/u31YJHO) at the time, small form factor embedded devices was our target platform.

The project would leverage Eris' smart contracts to govern five key areas:

 - Ownership of a device may be exchanged between users
 - Assignment of access rights to various components on a device (read, write, modify-permissions, etc.)
 - Configuration of device-to-device transactions
 - Management of device meta-data (e.g. hard-coding location data or linking up a GPS subsystem)
 - A system to log/broker data in bulk to 3rd party networks ("peering") optionally paying for data via a bitcoin oracle.


###Current Direction

My plan is to target Ubuntu-core (and Debian) running on small number of Beaglebone Black and/or Raspberry Pi devices - as well as mocks running on VMs and (time permitting) integration with less powerful Arduino compatible devices. 

To simplify matters, user accounts and access rights would be modeled after Unix style permission systems & linked to the OS's file system. An agent service with SUDO permissions would be used to modify the file system permissions in response to changes announced within the blockchain, and a [insert federated login system] will be used to bootstrap account surrogates. Access to components would be created through a named pipe (or similar mechanism) to allow for OS enforcement. 

Device to device communication and data encryption - while interesting - are likely beyond the scope of this project, however an effort will be made to ensure it is solution agnostic. I intend to create a quick and dirty SSH based system depending on how the federated logins end up working.

I would be doing regular write-ups on my progress with the goal of helping others to follow a similar journey. I am willing to do online talks and other promotional work as needed.


###Motivations

My motivations for a lot of what I do typically involve 3 key things:
 - My Mother: I want to help my disabled mother to be able to manage parts of her home from her bed.
 - Myself: I'm forgetful and want my house to help me do things. 
 - Mars: A robust distributed swarm of automated factories & farms on mars sounds like a cool thing to do.

I'm a big fan of OpenData initiatives and believe strongly in Free Open Source Software, Creative Commons, and Radical Transparency.  All this data we are generating should be given a chance to be free if people want it to be. I not see IoT (and by extension, the Quantified Self movement) getting big unless we conquer security, privacy, and ease of use concerns. I see Eris Industries' work being a key component of this vision. 

Or to put it simply: I hate the thought of a vendor owning my data, or the government knowing when I poop.

My wish is to inspire like-minded Makers (& Marmots) to get onboard with IoT and blockchain technology. I'd like to see the community working toward a system that makes it simple to get a device hooked up and start sharing in a secure way. 


###Why am I applying to an internship?

 1. I love this stuff.
 2. You might be willing to feed me so I can work on it.
 3. [I have no idea what I'm doing](https://twitter.com/ultimape/status/588302547376545793).
 4. I enjoy learning.


###Requirements / Costs

####One Time Costs
I would need a more functional computer. I believe I could make do with a Chromebook - I would be turning it into a dev machine along the lines of what [CodeStarter is doing for students](CodeStarter is doing for students). Prices range from $200-$400 for basic models unless you can get them on sale. For my purposes, the more ram, the better.

A bed would be nice and would greatly increase my productivity. I'd be happy with a futon mattress from Walmart/Overstock (only thing comfortable that will fit in my room). Cost ranges from $130-$300 depending on availability.

I would need a couple of IoT oriented embedded systems. Two would be the minimum for a proof of concept however I'd love to have a set of six. Two to act as IoT devices, three to act as extra nodes for the distributed server host, and one to simulate a 3rd party connection. So anywhere from $100-$500 depending on quantity, model, accessories and shipping costs. This includes components to integrate with hardware I already own.


####Monthly Reoccurring
There may be room at a local co-working space, which would run about $300 a month.

My current living arrangement has my rent set at 1/3 of my income. I am not sure if a stipend is counted, so that will need to be factored in.

I can live on $300 a month for food. I could go cheaper, but my current living situation leaves me without a lot of storage space and little ability to buy in bulk. I am not sure if I would be able to maintain my food stamps during the internship.

I believe my cellphone plan currently costs my little brother $20 - I'd like to cover that on my own.

Student loan debt collectors pull money out of my bank account each month, but I think it's only $5 right now. 


###Similar Projects

For similar projects in this space, refer to:

 - [@IBMIBV's ADEPT protocol](http://www.coindesk.com/ibm-reveals-proof-concept-blockchain-powered-internet-things/) - a yet to be finalized protocol proposal discussing a number of concerns. 
  - See a [demo at CES 2015](https://www.theprotocol.tv/adept-demo-ibm-samsung/).

 - [@Startstarad's TilePay ](https://twitter.com/Startstarad/status/578425604753747968) a management ĐApp.
   - focusing on monetization via what appears to be a coloured coin.
   - Seems to be aiming for the creation of a marketplace.
