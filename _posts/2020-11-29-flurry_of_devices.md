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

At the base of all our computational interactions we have everyday computing, with over x% of the population online on a personal device, we see that this has been growing quickly over the last years, online presence, social media, news and storing our important files are all integer parts of our modern lifestyles, no matter where we are on the planet, with services like LinkedIn, online banking and emergency hotlines computation and internet have become utilities of necessity. As we saw discussed in the last post, any modern smartphone or equivalent is enough to provide all of these, and a indepth introduction of mobile-desktops and my experiences with iPad OS and Samsung DeX is found here.


{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="For simplicity we can envision our personal computer as a common interface for itself and remote resources." %}

In fact, while we might not think of it, most of 'our' devices are not in our homes or office, they are represented as the enourmous and numerous server farms of cloud platform providers, from something as simple as file-syncing between devices and backups, to simulating economic models. Or the sheer scale of enterprise IoT in storage facilites and other automations, what we personally own is really just pees anyway, but there are a lot more of us potential IoT device owners out there, so it faces us with some grand challanges in protocol discovery, network topology and security. 

If we imagine the top of the line desktop would use 10h to compute one problem, then any other interaction in between would add to the total duration, in other words it is unavailable. Since these machines could easily use hundreds of hours to train deep neural networks, having the ability to inflate, to scale our work to another powerful node, or distribute it over many; if we lease cloud instances at 1m intervals, then hundreds of hours can be reduced to a single minute. This ability to produce results and test this quickly is can be essential, like sequencing a virus DNA and simulating vaccines to respond to a crisis. Just check our colab for how to use free GPU and TPU resources in the cloud.


{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="I don't know  about you, but I have never been fond of all the cables, the noise from disks and fans of using stationary computers, (hearing a gaming rig under load is like experiencing a plane perpetually take of besides you)." %}

Distributed computing introduces two new factors to consider, network bandwidth and latency, how many packages of data can we send at once, and how quickly do we get a respons from a request is made. Cloud gaming (or remotely operated robotics) are prime examples of this, the more sensitive our task is to small delays to our reaction time cloud computing might not always be our best bet. On my local network I achieve about 10-15ms with only the client over wifi (AC/AX) using parsec on a window host, from commercial solutions lice GeForce I have about 20-50ms depending on which network I was connected to (office, cafe or home), these are a small nuisance at best since you can even game with a free-tier on GeForce with lower graphics and resolution; now who says there's no such thing as a free lunch.

An important point for most users would be the associated costs of hosting yourself, or leasing from a clou
If we want high end graphics for the most recent titles we should expect a pricepoint of about 10-20$ a month, the graphics card alone of such a system might cost somewhere between 500-1000$ for the investment to be worth it, we would at the very least need to perform at that level for 25 months before replacing, that's not even considering the rest of the computer components. Low consumption users might find it differently, with a raspberry pi (rpi) 4b (less than 100$) or a simple core i3 SBC (about 250$ and up) can be enough to provide a cloud platform for everyday computing and some minor content creation. Leasing such an instance in the cloud would cost about 10-20$ monthly, and we can see how quickly our small investment pays off. There are some nice infrastructure features that we might wan't to account for before we can call it a true replacement, take a look here.

An interesting sidenote on the poetic justice of how we 'scale out' to use large centralized computers has become possible in large by how market segments like gamers and enthusiasts have made computer hardware improve quickly at competative prices, this was from a time when internet was either in its infancy, simple images could take minutes to load. Thus we scaled up our local machines to become ever stronger, faster, smarter devices, that in the end has been reduced to a thin client.
{: .notice--success}

As our computation became present 'anywhere', so did small wireless physical things pop up everywhere, from our toasters to automatic ticket systems. Ubicomp is about so much more than just getting the data we ask for on the device we're using, it is about using the hidden computation to gain and act on a context, to relieve us of extending our attention to the task. 

__*If the cloud is the brain, then IoT is the central nervous system.*__
{: .text-center}

It is an intricate combination of the small wireless things, pervasive in every aspect of our world, and 
 


Some commercial cloud gaming platoforms even offer free-tiers with limited session times (promts to login again) and reduced resolution and graphics; who says there's no such thing as free lunch.
{: .notice--info}

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="My DeX setup with a usb-c cable to the monitor for display, monitor usb hub and charghing my phone, using external drives and midi equipment is plug and play, no fans or spinning disks" %}

There is another positive aspect of having a computer that's always running in the background, we can get a context from all our devices and things gathered together, and besides the computers are the Internet of Things (IoT) which are can be a tiny microchip with wifi connection, which can be very cheap (the popular ESP chipset family is something we also use more here). They are usually not smart devices at all, and in general they have sensors to provide our system with context, and actuators that let us take action on it. How well an automation works, can be seen in terms of user attention it removes from a task, as we discussed in the last post it might be a flight itinirary, but turning of the light when no one is home, maybe starting the vacuumer if its not too late as well, we only need to be reminded when we should empty the bin. The smartness of these services lays in their ability to "predict" our preferences, a smart home is thus nothing without the brains. 


{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="New infrastructure, new possibilites" %}




In the next section we continue down the ladder to smart devices and the internet of things, and how to use them and much more to create a context for automation and synergy.




To understand our computational habits, I'd like to introduce three user groups, and the latter two is an extension of the first.
- Everyday computing: from emails, document collaboration, file management, social platforms and video streaming. 
- Content creation: it could be anything from creative content to coding and usually has two characteristics; discrete workloads and specialized work environments.
- Responsive computing: is the group of users that would need to interact with a remote desktop environment or otherwise, this is the case for VR chats, low latency gaming etc.



All developers, and most creative content creators can avoid the last group, responsiveness below 50ms isn't essential for most uses, on a local area network the difference in latency can be around 10ms, connections from outside would be additionally bottlenecked by upload capacities enforced by your ISP.
{: .notice--info}
