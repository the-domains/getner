---
inFeed: true
hasPage: true
inNav: false
inLanguage: null
starred: false
keywords: []
description: How the retail and infrastructure giant has subtly lead a massive change in how IT is organized.
datePublished: '2016-02-27T23:19:32.067Z'
dateModified: '2016-02-27T23:19:11.645Z'
title: The Amazon-ification of the Enterprise
author: []
authors: []
publisher:
  name: null
  domain: null
  url: null
  favicon: null
sourcePath: _posts/2016-02-27-the-amazon-ification-of-the-enterprise.md
published: true
url: the-amazon-ification-of-the-enterprise/index.html
_type: Article

---
Ever since I read [Steve Yegge's thoughtful "Platform Rant"][0] about his time at Amazon and specific frustration at Google, I have been fascinated by the this largely unreported, titanic shift in IT thinking that underlies all the buzzwords of 'Cloud', 'Apps', 'APIs' and 'X as a Service'. In my mind I think of it as the 'Amizonification' of the enterprise... but I'm sure there are catchier names.
![](https://the-grid-user-content.s3-us-west-2.amazonaws.com/aa32b250-e6db-47fe-87ba-72ad439edecc.png)

Origins of the Change 

I'll confess I don't know the exact pivot point when the shift occurred, and people can probably trace it to any number of similar events, but I think Yegge's exposition is one of the best sign posts. For those not wanting to read it, he details how when he was at Amazon Jeff Bezos decreed "All teams will henceforth expose their data and functionality through service interfaces". No ifs, ands, or buts. No exception. Period. Bezos didn't care what architecture you used, what OS, nothing that is the normal focus of most IT policy. He simply said that whatever project or function or system you were working on at Amazon was to delivered as a service to any other function. 

For technologists this may have seemed like either a good or bad idea, but likely viewed as capricious. I mean it you may have agreed to it, but the suddenness and absolute nature probably rubbed a lot of people the wrong way. For the business of Amazon however, and it turns out for IT of today, it is a seminal shift. 

For non-technologists, this deserves a bit more explaining. What Bezos did in one edict was say to all the different programmers, developers and project managers at Amazon that whatever project you are working on, it needs to accept input and deliver output in a standardized, structured way. Those inputs and outputs need to behave correctly whether that system or person interacting with your service was another Amazon system or something from half a world away. In other words, everybody talk to each other (digitally) in a very formal and structured way. While this may seem obvious to people who aren't engineers, this is not the way things are commonly done; mainly because it's not always the most efficient. For example, if you have a program that keeps track of all your client accounts, and a shipping system needs to access a client's address, the fastest way to do that is for the shipping program to look up the client's address in the account database. That works great and runs fast, but it also means that if the client account team wants to make any changes to that database they need to coordinate with \*all\* the users of that database. Let's say the company is U.S. focused and starts to market overseas. As a result you realize that the format of the postal code field has to change in order to accommodate different conventions in other countries. Now before you make the change you need to coordinate with any other service that is reading from or writing to your database to make sure they make corresponding changes to their system before you can make yours. 

You can imagine how quickly this becomes so complex that it becomes a real barrier to innovation. Systems become so intertwined that any change becomes months worth of cross-system negotiation. What Amazon changed was that, in our example, no one would get access to the client database. Instead now it would be the job of the client account system to respond to the request of the shipping system when it 'asked' for the client address. All reads of the database and writes to it go through a programatic service that the client system manages. All the client account team does is make sure it delivers the right information based on standard requests, and the details of how the system does that is irrelevant to the user of that information. It makes things a little more complex for the team working on the client account system, and takes a little more time for the shipping system to get a response vs directly accessing the database itself. So why do it? 

The answer is that by doing so, you decrease dependencies between systems and functions. If the client account team decides some new database system would be much faster or cost effective, they can change anything they want as long as their application still gives correct answers to requests from outside systems. Additionally, it now opens up the client account information to any of the existing or new business systems in Amazon. Let's say Amazon wants to test a new lawn care service. They can build an entire new service around scheduling and delivering lawn care, leveraging the client information they already have, and never have to bother the client account service team. Similarly, the shipping team can offer Amazon shipping services to 3rd parties, using the very same integration methods as they do with products shipped directly by Amazon. Both service areas can can expand their applicability, and integrate with new services with minimal impact on their core function. 

This is essentially how Amazon has gone from a book seller to the dominant player in providing infrastructure to effectively every dimension of the online world. They turned their data center management functions into services just as I described above, and then realized there were a lot more people out there interested in using data center resources and not managing them. Now Amazon Web Services (AWS) is almost interchangeable with 'cloud' with respect to enterprise IT. It has reshaped Amazon as a company, it has enabled the explosion of innovation in apps and services, and now it is fundamentally changing how the enterprise views IT. 

Enterprise Meet Amazon. Amazon Meet the Enterprise 

Even more profound than how this 'deliver as a service' philosophy has enabled the explosion of cloud services, is how it is changing traditional roles in technology and information. It used to be that the business defined requirements, IT helped source alternatives and then the team would select a vendor and implement. That worked for backup and archiving systems, email platforms, financial management packages and any other IT silo that was in the enterprise. Then one day someone started looking at 'the cloud'. Maybe it was the guys in charge of email, and they realized they might get better and cheaper email for the enterprise via a cloud vendor like Google or Microsoft. Maybe it was the sales team deciding that SalesForce was better than whatever internal system they had for CRM. Regardless, someone made the first move and now everyone is really thinking about information fundamentally for the first time in a long time. What exactly is the difference between a backup and an archive and aren't those so similar that they be integrated? If I want to integrate data from my CRM system into my product development research, should I really have to export and import data by hand into some separate system? Why the idea of outsourcing Customer Service so 'complex' but yet outsourcing the entire data center so simple. 

I don't mean to imply that no one ever thought about information before, but this amazon-ification of all of our preconceived notions is challenging many truisms of IT and information management. Users know that if they can get an app for virtually anything at home, then the company should be able to build similar apps to help them do their jobs. 

As enterprise IT becomes Amazon-ified you will see more and faster changes, including: 

* Custom-designed apps and services becoming a routine part of every business process, giving users information that exactly matches their desired work flow; 
* Seamless integration of cloud services with traditional behind-the-firewall systems, enabling selection of the best value solution regardless of location; 
* Increased speed of innovation within the enterprise, shifting enterprise IT into more of a development role that resource managers; and 
* An explosion of cross-enterprise business opportunities as business units are unshackeled to go where their markets guide them. 

Just something to think about the next time you buy a book at Amazon... If anyone still buys books at Amazon :-)

[0]: https://plus.google.com/app/basic/stream/z12ld3fwhlnexv5b004cjv0oapmuflzrezc0k