---
title: "Automate me: To ubiquity and beyond!"
last_modified_at: 2016-03-09T16:20:02-05:00
excerpt_separator: "<!--more-->"
header:
  image: /assets/images/ubi_header_1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com/@jesuskiteque)"
categories:
  - Blog
tags:
  - Ubiquitous-Computing
  - Automation
  - AutoLife
---
It might have been hard to imagine in 1988 just how pervasive computing would become today, with our myrad of personal smart gadgets and cloud services, even 30 years before the smart phone Mark Weiser lay forth a computer paradigm called Ubiquitous computing (ubicomp), in this era of calm technology, the computers themself fade unseen into the background. It is a paradigm born from how we design human-computer interfaces (HCI), and the context it provides our computations, it should make the data we would want or require available comfortably, as we move between home, office, hobbies and vacations. 

<!--more-->

The first wave of computing came with huge mainframes, these large and delicate machines could occupy everything from a room to whole factory floors, very often we coded with no operating system between the hardware and the users, the earlier versions was usually programmed with punching cards. These machines shrunk, their parts became robust and cheap, building and maintaince too; we entered the second wave of computing, the 'personal' computer. 
{% include figure image_path="/assets/images/computation-at-work.jpg" alt="devices in work environments" %}
If we look past the relative change in size, the big difference is that a pc is self contained with an operating system and files saved locally presented in an user interface (UI), this allows someone who knows nothing of computation browse cat pictures on the internet or create special effects for movies; we just need to know how to operate a screen with pointer and keyboard. Without going too deep into the technicalities, the desktop and laptop environments we are used to is part of the x86 CISC architecture, mobile devices popularily use ARM (Advanced RISC machines). While the ARM architecture was popular due to its higher return of computational resource over power consumption, the modern smartphone has come a long way since the iconic iPhone:

|name|cpu|ram|display|storage|camera|
| iphone 2G | 412mhz | 128mb | 3.5 inch 320x480 | 4-16gb | 1.92 mpx |
| samsung  s20 ultra | 2GHz octa-core | 12gb | 6.9 inch 1440x3200 | 128-512gb + microsd | 108mpx and more |

Between these devices stand nearly 13 years of improvements to smartphones, and maybe a more fair comparison would be between a laptop and a the modern smartphone, which we also explore in more detail in the next post. Over the same time period the [sales of smartphones](https://www.statista.com/statistics/263437/global-smartphone-sales-to-end-users-since-2007/) has multiplied by over a factor of ten, making it an equally big market share as desktops. This had huge impact on our day to day workflow, from emails, editing documents and collaboration, what our phones were too weak to handle on their own, we distributed to a cloud, today most users differenciate these platforms mostly on HCI, eg. a desktop has a monitor, keyboard and mouse and a windowed experience. It is only when we undertake more specialized tasks such as editing movies, developing code or even gaming that we notice the real differences, this is why most content creators use macos and gamers use windows or even propritary consoles.

{% include figure image_path="/assets/images/ecosystem.jpg" alt="a home-assistant dashboard" caption="A creative workstation and devices in a very propietary homogenous ecosystem." %}

These and other proprietary blockades is one of the main hampers to improving ubiquity, making specific services and ecosystems device dependent. As an example, the Apple TimeMachine backup feature is available on macOS devices, where you can use an external storage to make backups of all your personal data incrimentally, it is by far the best backup service I have tried for personal computers. And it is easy to understand that a person would continue to use this service, also considering you would always need a mac to open your backup.
So its only easy in so far as you keep bying from the same manufacturer, this even applies to new type of devices (eg. smart watch to phone compatability).
To some people this lack of control may have led them to think "No way I would accept that" or "I could do better myself", this stubborn denial to compromise is what I think is the proud backbone of todays vibrant open source communities. In fact, one of the most successful open source projects started out from just that with, Linus in his basement creating the first Unix kernel, the basis for Linux OS that today is the most widely used OS in the world, from mobile devices to supercomputers. Some projects are funded and provide steady realible updates and features, but like all diy projects they require some configuration.

{% include figure image_path="/assets/images/messy.jpg" alt="a home-assistant dashboard" caption="The mess hidden under the 'rug' from navigating multiple ecosystems." %}

The solution may not be open source or commercial exclusively, but a bit of both worlds. 
Commercial solutions often offer a lot of contextual automation out of the box, for instance using google as a mail provider and recieving a travel confirmation like for flights instantly creates an itinirary that tracks my journey. It offers a calculated departure time from my residence based on traffic estimates, and in the pandemic it even offers the most up to date regulations relevant for the trip. For most people, this convenience far outweighs the consequence of your flight information being visible to google; they probably knew if they wanted to anyway. Where an open source solution could benefit this is by letting us interact with the google itinerary, even from siri or alexa, open source projects are let us transgress proprietary walls with ease, and for most of its end consumers it is a way to increase functionality and even reduce costs and maintenance.
The AutomateMe repository and documentation reflects a lot of the features discussed here, and comes with modular service stacks pre configured to work together easily.

{% include figure image_path="/assets/images/autmation.jpg" alt="a home-assistant dashboard" caption="The mess hidden under the 'rug' from navigating multiple ecosystems." %}

The contextually aware services, often called automations is a key element to making computing ubiquitous by relieving the need for user attention, as in the example above where the correct information was used to produce a lot of handy information that I did not manually provide, the itinirary fluently available from my smartwatch to a desktop browser. This freedom from devices comes from the automation being run in a cloud, imagine it as a distribution of computers, some general-purpose nodes, some specialized for storage or machine learning. If we need more resources than on the local machine, or to preserve battery life distributing the workload to a remote environment where those resources are 'superflous' has enabled us to make almost any computation available at any device reliably; even cloud gaming and remote dekstops are viable options where some small delays are permittable. for me this has mostly resulted in playing CIV VI on the tablet from my couch.

So to conclude the first post in the automate me series, we should understand how the ubicomp paradigm wants us to provide contextually relevant data and behaviour, and that user attention is a valuable resource. For our everyday computing needs, the personal devices, from mobile to desktop is our preffered intereface, while specialised services are preferred for some mediums like TV for video content. How well our context is utilised is up to our ecosystem, or combination of them that we either bridge manually or extend with open source solutions. The next post looks closer at our personal and other HCI devices, their history and how they have changed together with our computational habits.

If you are interested in getting more hands on to improve your project or get started, go straight to my AutoLife documentation.
