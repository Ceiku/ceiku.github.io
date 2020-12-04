---
title: "Automate me: A flurry of devices"
excerpt_separator: "<!--more-->"
header:
  image: /assets/images/ubi_header_2.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com/@ranasawalha)"
categories:
  - automate me
tags:
  - Ubiquitous-Computing
  - Smart devcies
  - Cloud computing
  - Human Computer Interface
---
In 2020 every person world wide has on average 6 things connected to the internet, it is truly a flurry of computers, and things. From fitness trackers to server farms, understanding our habits and how it reflects our computational resource needs can both save us money as well as provide new features, imagine using one cable to turn your phone into a desktop computer, or a tablet that elegantly could double as a laptop, even providing you with end of the line desktop games on the go. 
<!--more-->

To understand our computational habits, I'd like to introduce three user groups, and the latter two is an extension of the first.
- Everyday computing: from emails, document collaboration, file management, social platforms and video streaming. 
- Content creation: it could be anything from creative content to coding and usually has two characteristics; discrete workloads and specialized work environments.
- Responsive computing: is the group of users that would need to interact with a remote desktop environment or otherwise, this is the case for VR chats, low latency gaming etc.

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="As VR offers higher immersion than on-screen content it provides a novel interface to do a lot of our everyday computing more intuitive, changing the playing field like the smartphone has done." %}

All developers, and most creative content creators can avoid the last group, responsiveness below 50ms isn't essential for most uses, on a local area network the difference in latency can be around 10ms, connections from outside would be additionally bottlenecked by upload capacities enforced by your ISP.
{: .notice--info}

At the base of all our computational interactions we have everyday computing, with over x% of the population online on a personal device, we see that this has been growing quickly over the last years, online presence, social media, news and storing our important files are all integer parts of our modern lifestyles, no matter where we are on the planet, with services like LinkedIn, online banking and emergency hotlines computation and internet have become utilities of necessity. As we saw discussed in the last post, any modern smartphone or equivalent is enough to provide all of these, read here for more on how I transitioned to using only my tablet and phone.

The content creators often need more horsepower, but they come in discrete loads, like compiling code or rendering a 3D model, lets say you wanted to train a neural net that would take your computer 2h, besides noise, we cannot exectly use the computer for other tasks without delaying our model training. If it also happened to be a laptop it would greatly drain our battery to work at such a high capacity, these issues dissapear when we distribute them, our personal device can still be used, and experience no extra power drain. There are a lot of ways to reduce the 2h wait time for the results, one is scaling up by getting a stronger machine, or scaling our into more machines in clusters, leasing from commercial solutions we could rent cloud instances at 1 minute increments and inflate to 120 on demand. For some business this ability to respond quickly to changes can be essential, for the rest of us, it depends on how many hours it is used before we need to replace.

Responsive computing differs from content creators that had discrete workloads, responsive computing has interactive sessions where latency can be crucial, for remote robotics or cloud gaming the delay experienced as data travels between the nodes can impair our performance. The only end consumers who really need to consider this category are computer gamers, often FPS and online high paced PVP games. 


As we continue to talk about servers, it can be nice to visualize them as 'headless' desktops, there is no screen, often no support for graphics at all through the OS. This saves us a lot of resources on the server, and instead we can imagine that the 'headed' part of the device is common for both the server and client, that takes care of visualizing and interfacing with the user.
{: .notice--info}

This change of perspective lets us view personal computers through their human-computer interfaces like, screen-realestate (a combination of dimension and pixel densisty), periphirals like touch/pen input, windowed experience or multiple monitors. While a tablet and a laptop might share the same segment of screen realestate, their periphirals makes them suited to different parts of document editing, keyboard and mouse is often preferred for longer writing sessions or bigger projects. Overlapping devices such as this tend to be a costly affair if we want them both to have quality displays, gamers might struggle between their home rig, and their laptop. 

Fewer devices frees up assets, we could get higher performing devices instead, or buy those things we otherwise would not afford, to know when to buy and lease power for our cloud can be a bit tricky. If we want high end graphics for the most recent titles we should expect a pricepoint of about 10-20$ a month, the graphics card alone of such a system might cost somewhere between 500-1000$ for the investment to be worth it, we would at the very least need to perform at that level for 25 months before replacing, that's not even considering the rest of the computer components. Low consumption users might find it differently, with a raspberry pi (rpi) 4b (less than 100$) or a simple core i3 SBC (about 250$ and up) can be enough to provide a cloud platform for everyday computing and some minor content creation. Leasing such an instance in the cloud would cost about 10-20$ monthly, and we can see how quickly our small investment pays off.

Some commercial cloud gaming platoforms even offer free-tiers with limited session times (promts to login again) and reduced resolution and graphics; who says there's no such thing as free lunch.
{: .notice--info}

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="My DeX setup with a usb-c cable to the monitor for display, monitor usb hub and charghing my phone, using external drives and midi equipment is plug and play, no fans or spinning disks" %}

There is another positive aspect of having a computer that's always running in the background, we can get a context from all our devices and things gathered together, and besides the computers are the Internet of Things (IoT) which are can be a tiny microchip with wifi connection, which can be very cheap (the popular ESP chipset family is something we also use more here). They are usually not smart devices at all, and in general they have sensors to provide our system with context, and actuators that let us take action on it. How well an automation works, can be seen in terms of user attention it removes from a task, as we discussed in the last post it might be a flight itinirary, but turning of the light when no one is home, maybe starting the vacuumer if its not too late as well, we only need to be reminded when we should empty the bin. The smartness of these services lays in their ability to "predict" our preferences, a smart home is thus nothing without the brains. 


{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="New infrastructure, new possibilites" %}




In the next section we continue down the ladder to smart devices and the internet of things, and how to use them and much more to create a context for automation and synergy.


