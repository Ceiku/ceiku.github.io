---
title: "Automate me: In a flurry of devices"
last_modified_at: 2016-03-09T16:20:02-05:00
excerpt_separator: "<!--more-->"
header:
  image: /assets/images/ubi_header_2.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com/@ranasawalha)"
categories:
  - Blog
tags:
  - Ubiquitous-Computing
  - Automation
  - AutoLife
---
It might have been hard to imagine in 1988 just how pervasive computing would become today, with our myrad of personal smart gadgets and cloud services, even 30 years before the smart phone Mark Weiser lay forth a computer paradigm called [Ubiquitous computing](https://www.lri.fr/~mbl/Stanford/CS477/papers/Weiser-SciAm.pdf) (ubicomp), in this era of calm technology, the computers themself fade unseen into the background. It is a paradigm born from how we design human-computer interfaces (HCI), and the context it provides our computations, it should make the data we would want or require available comfortably, as we move between home, office, hobbies and vacations. 

<!--more-->


As we touched upon in the last post, we tend to have a lot of devices, often they provide some common basic tasks such as everyday computing (files, web, documents and mail) while we do these tasks on both a phone and a computer they vary greatly, the phone is battery powered, has cellular and gps. The desktop in turn potentially has multiple big monitors, a keyboard and mouse. We can find it helpful to distinguish these and the catogries in between such as laptops in terms of:
- screen-realestate (sr): a combination of the physical dimensions and pixel density.
- periphirals: inputs like touch and keyboard, or outputs like sound and haptics.
- operating system: the interface between our physical components and users.
- hardware: both architecure (ARM vs amd64) and features (camera, battery, cellular etc)

The most common device is the phone, comparing the number of features, compact size and computational resource to their price, no other appliance or device even compares, making it the most persvasive general computing platform in the modern world. So the most important device to adress has a relatively small screen-realestate, it relies primarily on touch as input and uses the ARM architecture. 

**The thing about amd64 and ARM architectures is they developed to address two very different needs, the x86 (now amd64) was an architecture made for larger systems where we could supply more power, ARM systems made its way into the little things. Flash forward to today, and the little things have ample power to do a lot of the tasks we only designed for x86. Though this is changing lately, MS surface is a tablet with amd64 architecture, that provided a full desktop and hybrid tablet experience. Apple has gone the other way and revealed their next line of macbooks to sport ARM chips in a laptop format, the lines separating the two are getting blurrier, adding to the increasing trend to run our computations remotely the distinction between the two seem to matter less.

Maybe coupled with a TV for a screen for comfortably viewing movies etc, these user have no need to do more document work than look over some details and emails, and represents the simplest user device typology.

"phone img"

This is not saying they never use a computer, if they need it in a professional sense, chances are their employer would provide it too, it is not a personal device. But some users also need something more, it could be a tablet for binging series in bed, or sketching scenary, even 3D models, maybe a computer to play games, a laptop if they want to game at gatherings with friends too. 

"phone comp img"



In fact most the users on the internet do so from a phone, using our finger to click drag and pane our way throug digital information both from the couch or on the move, for many users this is more than enough, maybe paired with a smart tv or a gaming console. If they need a computer in a profesional sense, then this is usually provided for at the office. 

The second group usually expand due to two reasons:
- screen-realestate,
- architecture or OS, 

In the case of architecture it is usually access to creative tools (3D, photo, video) or with gaming that is somewhat restricted to Windows OS that are the reasons we get a computer, so it is for specialised tasks. Screen-realestate is often solved with a tablet, or a TV/monitor, 

is second nature.

In contrast it us usually not a good platform to multitask between many applications since we have no window manager, writing and editing large documents become tedious with the on screen keyboard. 


If we take a look at my topology of computers and mobile devices at home just a few years ago before I started my degree in computer science:
- phone: android
- tablet: ios
- laptop: macOS
- desktop: Windows
- server?: raspberry pi (raspbian)

So that means five different operating systems (OS), varying types of ARM and amd64 architectures, it was becoming a bit cumbersome to use all my devices, the tablet became a backup to the laptop for a bedside screen, the raspberry became a time-capsule with my external drive connected that would break every now and then, eating up my attention to do maintenance. After I finished my degree and fell into the home office rythm that we have during the pandemic I found myself with some time to do some digital "renovation", a sneak peak at my deployment today:
- phone: android (dex)
- tablet: ipad OS
- server: 2x older i3

Earlier this year I had an accident with my old and trusty phone, and with the US-Chinese embargo in heat I was looking for a non chinese brand, and I discovered samsung dex, a desktop environment from your phone with a single cable. I decided to give it a spin, with the thought that if I could game the few titles I occationally play with cloud computing, I would just sell my stationary; and boy was it good enough. As far as an desktop operating system it still has ways to go, but from intuitive keybinding on full mouse and keyboard support to file managing, even on connected drives or networking can be done here. I didn't sell my monitor, which with one usb-c cable both charges my phone, gives it access to the screen and usb hub for dex, alternatively you can connect it to an exisiting computer with a client app and "take over" which is great if you want to keep your desktop configuration wherever you are. Not too long after the campus goes into lockdown and I had to present my lectures in math and physics using video conferencing tools, and got an iPad pro for all my professional work, for my studies I had used the phone both at the lab and home desktop stations to build my artifact and write the thesis. Besides coding I also used my mac for a range of creative content development like music with garageband, 3D models with blender, even some photo and video work in adobe, but I hardly used their full toolkits and noticed the iPad OS versions to offer close to, if not the same functionality

Since I worked as a lecturer in math and physics alongside my studies, I had to find an alternative for the classroom whiteboards for sketching and equations from home and I got an iPad pro 
To understand what happened to the stationary and laptop computer (desktop environments) lets separate the desktop environments into headed (like windows and macOS that provide a graphical interface) or headless (a console interface only), thinking of the headed OS as making it a "personal" machine. 

Headless configurations does not use any resources on providing this interface, which is usually great for servers where we usually interface over command line anyway.






this is not including smart watch, consoles or other devices, just backing up and configuring all these devices became a nuisance and more maintenance than I liked, not to mention hardware upgrades on so many devices and service subscriptions easy become a piling cost. 

It is not that we use less computational resource, we just interact with it differently, by allowing an email provider  The notion of user attention as a resource is important,

while the desktop segment still has a hold on specialised services gaming and advanced creative tools, the "personal" in PC is dead.

 This boom in power over price and size had an impact in all fields of computing, and now the average person har (()) devices and we have on average (()) IoT devices, this impressive amount of data has the potential to provide unprecedented context. Allowing an email provider to automatically set an itinirary upon recieving a booking confirmation email for a flight, it uses its map service to compute estimated depature times from my home or hotel address seamlessly, freeing the users attention from the need of any device or notebook to stay ahead on their trip. While it is an impressive use of context, other mail providers have equally context aware features, but they differ based on their proprietary ecosystem. Besides automations such as the itinirary example, general computing software and files have historically been incompatible and in constant rivalry, often to the loss of end users (ms office vs apple works?), cloud document suites have long since made that notion obsolete, more recent examples is the IoT and cloud standards. This level of computation reached ubiquity, which is not saying that we comfortably edit excel sheets on our smartwatch, but devices with adequate screen realestate and peripherals (touch is often enough for light editing, keyboard and mouse otherwise) all present the relatively the same features.

In this comparison of units sold in the mobile and desktop market segments between yy we see that the mobile market is far bigger and growing in relative share, while the desktop segment still has a hold on specialised services gaming and advanced creative tools, the "personal" in PC is dead.
We still use just as much computational resource, just "distributed" differently
