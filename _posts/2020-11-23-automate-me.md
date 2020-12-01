---
title: "Automate me: To ubiquity and beyond!"
last_modified_at: 2016-03-09T16:20:02-05:00
excerpt_separator: "<!--more-->"
header:
  image: /assets/images/ubi_header_1.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com/@jesuskiteque)"
categories:
  - automate me
tags:
  - Ubiquitous-Computing
  - Cloud computing
  - Human Computer Interface
  - Automation
---
It might have been hard to imagine in the 80's just how pervasive personal computers would become today, with our myriad of personal smart gadgets and cloud services, in 1991, about 15 years before the smart phone, Mark Weiser lay forth a computer paradigm called [Ubiquitous computing](https://www.lri.fr/~mbl/Stanford/CS477/papers/Weiser-SciAm.pdf) (ubicomp), in this era of calm technology, the computers themself fade unseen into the background. It is a paradigm born from how we design human-computer interfaces (HCI), and the context it provides our computations, it should make the data we would want or require available comfortably, as we move between home, office, hobbies and vacations. 

<!--more-->

The first wave of computing came with huge mainframes, these large and expensive machines could occupy everything from a room to whole factory floors, very often we coded with no separation between the hardware and the user (the earlier versions was usually programmed with punching cards). These machines shrunk, became more efficient and for the same cost, by the 80s we entered the second wave of computing, the 'personal' computer. 
{% include figure image_path="/assets/images/computation-at-work.jpg" alt="devices in work environments" %}
If we look past the relative change in size, they came with operating systems (OS) that in the beginning only provided simple commands and file management, developed to have pointing interfaces such as the mouse and (touch) screens. These developments allowed computers to become personal, as we needed to know less about how the machinery work, the user interfaces (UI) is the same wether we are browsing images of cats, creating special effect animation, or even simulating black holes. The only thing we need to learn about the two common [architectures for general-purpose computing](https://cs.stanford.edu/people/eroberts/courses/soco/projects/risc/risccisc/), RISC (ARM) and CISC (x86), is that generally they represent the mobile and desktop markets respectively. The ARM architecture has traditionally been popular in mobile devices due to its higher return of computational resource over power consumption, and was usually quite weak devices, though a lot changed since the iconic iPhone:

| year |name|cpu|ram|display|storage|camera|
| 2007 | iphone 2G | 412mhz | 128mb | 3.5 inch 320x480 | 4-16gb | 1.92 mp |
| 2013 | HTC One | 1.7ghz quad-core | 2gb | 4.7 inch 1080x1920 | 32-64gb | 4mp
| 2020 | samsung  s20 ultra | 2ghz octa-core | 12gb | 6.9 inch 1440x3200 | 128-512gb | 108mp (array) |

Between these devices stand 13 years of inovation, it is a perfect example of moore's law at work, but that's not the whole reason why, the power we could squize into our pockets just kept increasing, and as updates kept coming [we kept bying](https://www.statista.com/statistics/263437/global-smartphone-sales-to-end-users-since-2007/) and the sales have increased tenfolds over this time, making it an equally big [market share](https://gs.statcounter.com/platform-market-share/desktop-mobile-tablet/worldwide/#monthly-200901-202010) as desktops.
For many reasons the smartphone revolutionized HCI, it made general computing, well generally available to anyone, now they have enough power to be compared with a low to mid range laptop. But there are some tasks where these machines still haven't managed to become useful, when writing long documents it is nice to have a keyboard or a windowed experience to multitask. So even though phones have historically offered some degree of monitor and periphiral support (keyboard and mouse), it is only very recently with Samsung DeX and iPad OS we're starting to see real innitiative towards mobile-desktop hybrid OS; MS surface is another example where the desktop environment is delivered in a tablet formfactor.

The reason why we would hardly notice the switch (and tablet computing is trending) is that most of our tools and files now exist in the cloud, as end consumers we only need to store personal or sensitive data locally or encrypted. Even as a developer I code everything on a cloud-platform, all my tools are available on any device with a web browser, which is why I got rid of my stationary and laptop that saved money, reduced noise from fans and disks and gave me access to any service anywhere; kind of. It is not an unknown problem to become "plaform dependent" however, eg. Apple TimeMachine backup feature is available on macOS devices, where you can use any external storage to make backups of all your personal data incrimentally, it is easy to use and has a good interface; it is easy to understand that someone would keep bying the same platform. So its only easy in so far as you keep bying from the same manufacturer, this even applies to new type of devices (eg. smart watch to phone compatability).
This has become proprietary walls to our ubuquitous dream, but some people just don't do that kind of compromise.

{% include figure image_path="/assets/images/ecosystem.jpg" alt="a home-assistant dashboard" caption="A creative workstation and devices in a very propietary homogenous ecosystem." %}

To some people this lack of control may have led them to think "No way I would accept that" or "I could do better myself", this stubborn denial to compromise is what I think is the proud backbone of todays vibrant open source communities. In fact, one of the most successful open source projects started out from just that with, Linus in his basement creating the first Unix kernel, the basis for Linux OS that today is the most widely used OS in the world, from mobile devices to supercomputers. Some open source projects are funded and provide steady realible updates and features, but unlike most commercial solutions they require some configuration, beyond that they provide a equal (sometimes more) features as paid solutions.

{% include figure image_path="/assets/images/messy.jpg" alt="a home-assistant dashboard" caption="The mess hidden under the 'rug' from navigating multiple ecosystems." %}

Perhaps we don't want to replace everything, no need to re-invent the wheel. 
Commercial solutions often offer a lot of contextual automation out of the box, for instance using google as a mail provider and recieving a travel confirmation like for flights instantly creates an itinirary that tracks my journey. It offers a calculated departure time from my residence based on traffic estimates, and in the pandemic it even offers the most up to date regulations relevant for the trip. For most people, this convenience far outweighs the consequence of your flight information being visible to google; they probably knew if they wanted to anyway. Where an open source solution could benefit this is by letting us interact with the google itinerary, even from siri or alexa, open source projects are let us transgress proprietary walls with ease, and for most of its end consumers it is a way to increase functionality and even reduce costs and maintenance.
The AutomateMe repository and documentation reflects a lot of the features discussed here, and comes with modular service stacks pre configured to work together easily.

{% include figure image_path="/assets/images/automation.jpg" alt="a home-assistant dashboard" caption="The mess hidden under the 'rug' from navigating multiple ecosystems." %}

The contextually aware services, often called automations and is a key element to making computing ubiquitous, by relieving the need for user attention, as in the example above where the correct information was used to produce a lot of handy information that I did not manually provide, now on any device. This freedom from devices comes from the automation being run in a cloud, imagine it as a distribution of computers, some general-purpose nodes, some specialized for storage or machine learning. If we need more resources than on the local machine, or to preserve battery life distributing the workload to a remote environment where those resources are 'superflous' has enabled us to make almost any computation available at any device reliably; even cloud gaming and remote dekstops are viable options where some small delays are permittable. 

To conclude the first post in the automate me series, we should now understand how the ubicomp paradigm wants is aimed to provide contextually relevant data and behaviour, and that user attention is a valuable resource in doing so. For our everyday computing needs, the personal devices, from mobile to desktop is our preffered intereface, while specialised services are preferred for some mediums like TV for video content. How well our context is utilised is up to our ecosystem, or combination of them that we either bridge or extend with open source solutions. The next post looks closer at our personal and other HCI devices, their history and how they have changed together with our computational habits, and if you are interested in getting more hands on to improve your project or get started, go straight to my [AutoLife documentation](https://ceiku.github.io/AutoLife/).
