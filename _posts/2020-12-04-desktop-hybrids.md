---
title: "Mobile desktops, just a hybrid?"
last_modified_at: 2016-03-09T16:20:02-05:00
excerpt_separator: "<!--more-->"
header:
  image: /assets/images/ubi_header_1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com/@jesuskiteque)"
categories:
  - workflow
tags:
  - Ubiquitous-Computing
  - Cloud computing
  - Mobile devices
  - Coding
  - Human-Computer Interface
---

Computers are expensive, our budget is split over mobile and desktop devices to provide us with comfortable interfaces for our needs, from working on documents or 3D files, or entertainment with games and binging series. On a limited budget getting the features we want become hard, and we might wish that our tablet and laptop was reduced to one device.

<!--more--> 

This is where mobile desktop hybrids enter the market, and combined with distributed computing we can for the most part have our services and data on any device, any where. This has meant that users on a low budget has been edging for more ways to use their phones and tablets, with periphiral support for mouse and keyboard we come a long way to provide the same comfort in editing larger documents etc as a desktop. Besides 'everyday' computing, the computer is a tool with a lot of specialized hardware and software for advanded data manipulation, they also provide a windowed experience that can stretch over any and multiple monitors.

This has changed a lot, and with a little bit of McGyver magic they are hardly distinguishable.
To help this story along, I will use my own transistion as a lecturer, coder (anything from micro controllers to machine learning) and the content creation I do on my spare time (record and jam sessions, green screen video and 3D modelling) from being platform dependent to independent.

I had a desktop with a dedicated GPU that I got mainly for gaming, but the GPU quickly found other uses too, it was a mid-range computer with enough power to pull 

In my long list of devices I had a stationary that was my trusted mid range gaming rig, a mid range android phone and an iPad mini for garageband and movies while out and about. As I started my degree I also got a macbook pro, flash forward about five years, to 2020 I had to provide my students with online classes, with math and physics, a proper whiteboard is essential; so I got an iPad pro with the pen.

The new iPad quickly became a stable tool in my creative workflows, sketching and 3D modelling became a breeze, but I started to feel encumbered by my devices. The few days I still had at the office or lab required me to bring two devices, nearly the same dimensions to and from work, I also had to unlock and switch focus between devices (luxury problems), and files still had to be synchronized between them too.

At home I had even more devices to switch between, from gaming, to just checking a few notifications on social media, I felt split between devices to charge, or that was plugged into the wall. So I had my first moment of stubborn appiphanies, 'why not just run the stationary as a server?': no more file synching, no more device juggling. To get a feeling of the problems we face when setting up our own cloud platform, how to assess the expenses, or how much we will save, head over on over here.

As a developer, my first instinct in doing so was "there's gonna be no way I can work on my tablet as though it was my mac" but boy was I wrong, VS code had plans to rock my world yet again, we can either use their commercial solution, or just host our own VS code IDE through webviews! Everything from linting and extensions was present (some extensions, mainly previews like web or latex are still underway), but with a terminal those problems just seem trivial. An important feature here is that the main network consumption is by sending text files forth and back the heavy lifting is done elsewhere, this greatly increases battery life and makes long sessions over cellular fade in comparison to those two youtube clips you watched during the break; personally I have tested working away from home on a two day hike with my tablet and a small powerbank (10Ah) and came home with plenty of juice left and under 100MB of 4G data consumed. 

My macbook that cost over twice of my iPad with its keyboard folio and pen, which had now replaced it for all intents and purposes, the noisy big computer at home was all I needed to provide an ubiquitous interface. The second strike came when I needed to upgrade my phone, it was around the time where I had gotten curious about Samsung DeX as well (coincidence?), and while I loved the ipad my sessions on the go, I still missed the truly windowed experience that my stationary provided at home for long session. This is what DeX attempts to do, and honestly the only difference is the lack of multi-monitor support; which I hear is coming anyway. 

Unlike iPad OS, Android already have a lot of UNIX tools that developers might know, apps like termux gives us a terminal that can do almost anything short of containerisation like docker, we can host our web servers for local development for moments we cannot connect to our cloud platform; it is the closes to a standalone mobile-desktop hybrid that I have tried. Both hybrid OS provide filemanagers, we can use external drives (usb hubs are essential for mobile devices as computers), keyboard and mouse support is present, but the pointing overlay for iPad OS still has some issues to iron out (like scrolling in webviews).

So far we have discussed how the mobile devices can replace our desktops, but this leaves out half the story, where mobile devices are fundamentally different, when it comes to social media, sharing, notifications and navigating with maps, our mobile devices come packed with hardware and apps to meet our needs, these are interwoven into these hybrids in a way that makes contextual sense. If we were to demand a laptop with 5G, multiple cameras (say 100mp on the main lens), day long battery life, gps and all the other things we have in our smartphones the pricetag might make us cry a little, so why look further than mobile.
