#Nicholas Perry ([@ultimape](https://twitter.com/ultimape))'s Project Proposal:

##Project Hephaestus [?](http://en.wikipedia.org/wiki/Hephaestus#The_craft_of_Hephaestus)

###A Maker oriented proof-of-concept Internet of Things (IoT) network showcasing Eris Industries' systems. 

The main goal of this project is to create a simple monitoring/control website running on top of Eris's Decerver that is able to interact with IoT devices. Eris's blockchain tech will also be used to manage the exchange (transaction) of messages between various sensors, displays, and actuators. The proof-of-concept should allow for a decentralized way to manage a large (and distributed) 'Internet of Things'.

The project is a security minded modernization of my senior project team's '[smartHAuS](https://docs.google.com/presentation/d/1tgCkLdP88__5RmmTR4XizIDXYIWXTe-LuWtThk_1CRc/edit?usp=sharing)' originating out of my degree work at Vermont Technical College. I will also be taking heavy influence from a subsequent project I was developing at Praetor Labs internally known as [Shardonnay](https://workflowy.com/s/493ab350-f171-d9c0-6ef1-f50c68ca65a6). It ended up having a distributed resource model as our primary goal. While we were using [a cluster of ShuttlePCs](http://imgur.com/u31YJHO) at the time, small form factor embedded devices was our target platform.

Like my senior project's goal, the hope is to have the system be painless to setup for a hypothetical tech illiterate home-user (a.k.a. my dad).

The project would leverage Eris based smart contracts to govern five key areas:

 - Ownership of a device may be exchanged between users
 - Assignment of access rights to various components on a device (read, write, modify-permissions, etc.)
 - Configuration of device-to-device transactions
 - Management of device meta-data (e.g. hard-coding location data or linking up a GPS subsystem)
 - A system to log/broker data (in bulk?) to 3rd party networks ("peering") optionally paying for data via a bitcoin oracle.


###Current Direction

My plan is to target Ubuntu-core (and Debian) running on small number of Beaglebone Black and/or Raspberry Pi devices. It may also include service mocks running on VMs and (time permitting) integration with less powerful Arduino compatible devices. The system would nessisarily include a small sample of IoT style usecases. 

To simplify matters, user accounts and access rights would be modeled after Unix style permission systems & linked to the OS's file system. An agent service with SUDO permissions would be used to modify the permissions in response to changes announced on the blockchain, and a [insert federated login system] will be used to bootstrap account surrogates. Access to components would be created through a named pipe (or similar mechanism) to allow for OS enforcement. 

Device to device communication and data encryption - while interesting - are likely beyond the scope of this project, however an effort will be made to ensure it is solution agnostic. I intend to create a quick and dirty SSH based system depending on how the federated logins end up working.

I would be doing regular write-ups on my progress with the goal of helping others to follow a similar journey. I am willing to do online talks and other promotional work as needed.

----

###Motivations


My wish is to inspire like-minded Makers (& Marmots) to get onboard with IoT and blockchain technology. I'd like to see the community working toward a system that makes it simple to get a device hooked up and start sharing in a secure way. 

My motivations for a lot of what I do typically involve three things:
 - My Mother: I want to help my disabled mother to be able to manage parts of her home from her bed.
 - Myself: I'm forgetful and want my house to help me do things. 
 - Mars: A robust distributed swarm of automated factories & farms on mars sounds like a cool thing to do.

I'm a big fan of OpenData initiatives and believe strongly in FOSS, Creative Commons, and radical transparency.  All this data we are generating should be given a chance to be free if people want it to be. I do not see IoT (and by extension, the [Quantified Self movement](http://www.brookings.edu/research/reports2/2014/09/cyborg-future-law-policy-implications)) getting traction in the home market [unless we conquer security, privacy, and ease of use concerns](http://a16z.com/2015/01/08/a16z-podcast-the-technology-is-ready-so-where-is-the-internet-of-things/). I see Eris Industries' suite of tools being a key component of this vision. 

Or to put it simply: I hate the thought of a vendor owning my data, or the government knowing when I poop.


###Requirements / Costs

I am quite frugal and would be willing to work on the project (and other duties) for very little. Although, I would need to aquire a couple of items if I were to comit to this for 8 - 12 week. I've broken down the costs below:

| Monthly? | Need? | Cost | What | Reasoning |
| :---------: | ---: | :--- | :-----: | :----- |
| yes | yes | $300 | Co-Working Space | I may have access to a co-working space in town. Much better working environment that my cramped bedroom. |
| yes | yes | $300 to ??? | Rent | Rent is 1/3 of my income per current living arrangments. |
| yes | yes | $300 | Food | If I could live off of Soylent, I would. |
| yes | yes | $20 | Taxables | I need to make sure I have deoderant and other hygiene items.
| yes | yes | $5 | Student Loans | Hooray, student loans. :/ |
| yes | maybe | $50 | Travel | Time in Burlington for collaborating with the [local hackerspce](http://laboratoryb.org) would be helpful. |
| yes | no | $20 | Phone | Currently being covered by my little brother. |
| no | yes | $200 to $400 | Computer (chromebook) | To turn into a [dev-machine](blog.codestarter.org/post/93985346780/how-we-turn-199-chromebooks-into-ubuntu-based) as my current laptop is awful. |
| no | yes | $100 to $500 | Embedded Systems | Two (minimum) to six ( for 100% standalone system) embededed linux boxes to create proof-of-concept system.  |
| no | kinda | $130 to $300 | A bed | A futon matress so I don't have to sleep on the floor will greatly improve productivity. |

###Nice-to-haves

Not really a requirement, but I could use some things to help with branding when sharing the project in public:

| Cost | What | Reasoning |
| :--- | :-----: | :----- |
| $100 | Hair-dye | Green hair-dye to assist with branding. People remember green hair and it is useful for attracting attention. |
| $20 | [Marmot](http://smile.amazon.com/Folkmanis-3034-Groundhog-Hand-Puppet/dp/B00KWJZHEI/) | A little marmot friend to act as a mascot. It might end up part cyborg. |
| $20 | Eris T-shirt | A black t-shirt would be best as I would be [modifying it](http://www.instructables.com/id/T-shirt-Designs-with-Stencils-and-Bleach/) to go along with the Maker motif. |


###Why am I applying to an internship?

 1. I love this stuff.
 2. You might be willing to feed me so I can work on it.
 3. [I have no idea what I'm doing](https://twitter.com/ultimape/status/588302547376545793).
 4. I enjoy learning.
 5. [Proof of Cuddle](https://twitter.com/hashtag/proofofcuddle) should be a thing.


###Similar Projects

For similar projects in this space, refer to:

 - [@IBMIBV's ADEPT protocol](http://www.coindesk.com/ibm-reveals-proof-concept-blockchain-powered-internet-things/) - a yet to be finalized protocol proposal discussing a number of concerns. 
  - See a [demo at CES 2015](https://www.theprotocol.tv/adept-demo-ibm-samsung/).

 - [@Startstarad's TilePay ](https://twitter.com/Startstarad/status/578425604753747968) a management ĐApp.
   - focusing on monetization via what appears to be a coloured coin.
   - Seems to be aiming for the creation of a marketplace.
