---
title: "Automate me: In a flurry of devices"
last_modified_at: 2016-03-09T16:20:02-05:00
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
In 2020 every person world wide has on average 6 things connected to the internet, it is truly a flurry of devices and things from fitness trackers to desktop computers. Understanding our habits and computational resource needs can both save us money as well as provide new features, imagine using one cable to turn your phone into a desktop computer, or a tablet that elegantly could double as a laptop, even providing you with end of the line desktop games on the go.
<!--more-->

To understand our computational habits, I'd like to introduce three user groups, and the latter two is an extension of the first.
- Everyday computing: from emails, document collaboration, file management, social platforms and video streaming. 
- Content creation: it could be anything from creative content to coding and usually has two characteristics; discrete workloads and specialized work environments.
- Responsive computing: is the group of users that would need to interact with a remote desktop environment or otherwise, this is the case for VR chats, low latency gaming etc.

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="As VR offers higher immersion than on-screen content it provides a novel interface to do a lot of our everyday computing more intuitive, changing the playing field like the smartphone has done." %}

All developers, and most creative content creators can avoid the last group, responsiveness below 50ms isn't essential for most uses, on a local area network the difference in latency can be around 10ms, connections from outside would be additionally bottlenecked by upload capacities enforced by your ISP.
{: .notice--info}

At the base of all our computational interactions we have everyday computing, with over x% of the population online on a personal device, we see that this has been growing quickly over the last years, online presence, social media, news and storing our important files are all integer parts of our modern lifestyles, no matter where we are on the planet, with services like LinkedIn, online banking and emergency hotlines computation and internet have become utilities of necessity; to some degree a any smartphone would do. From editing big excel sheets and writing long documents with a desktop environment, to navigating the streets of a new city while talking to a friend back home on the phone, their difference in HCI like screen realestate, input methods and periphirals makes them comfortable tools to different aspects of our digital lives. Some hybrid devices that challenge these boundraries exist in both direction, the chromebook is a tablet-laptop with the HCI of a laptop with the mobile architecture, on the other hand the ms surface is a laptop-tablet that comes as a tablet with laptop hardware. Together with Samsung DeX that is all the desktop experience casual users would ever need packed into your phone, for now we may have to do without multi monitor support. Apple has also made some steps in this direction, with the magic keyboard folio for select ipad models and ipad os they have made big steps towards creating very good hybrids for creative content, more on both of these here.

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="My DeX setup with a usb-c cable to the monitor for display, monitor usb hub and charghing my phone, using external drives and midi equipment is plug and play, no fans or spinning disks" %}

In fact, where tablets offer the same screen realestate as laptops, and a touch interface that couples well with a pen for sketching, it also comes with cellular and other features seldom found in their laptop counterparts, the desktop phone combo gives the most common device all the utilities to remove the need for a desktop computer all together. Our next challenge is to provide a ubiquitous interface to all our computational services, resource demanding or centralized tools may be presented in webviews such as the code-server that hosts a full Visual Studio Code IDE as a webview. This strategy has a low impact on network bandwidth as only requested files and their changes are sent between the client and server, where it can be compiled and run. It is the same for someone rendering a 3D model, their tablet or phone is suffiecient to present and interact the data, the selected operations can then be handled remotely to perserve battery life; but a modern android phone has the language packs popular languages and a unix shell with termux so we could perform a lot of our workflow locally, the android kernel lacks some features such as containerisation however.

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="New infrastructure, new possibilites" %}

At one my most device riddled point I had my phone, a work laptop and tablet, and a gaming desktop, keeping these devices up to date is a big expense, and now that my phone has taken over for my desktop, and my tablet doubles in as a laptop with its keyboard folio, selling the superflous devices (also the most expensive ones) freed up a lot of assets and saves me from future investments like it. In fact even for specialized usage like gaming, if we can manage a 20-30ms delay difference we can save a lot of money from commercial solutions, some even offer free-tiers with limited session times (promts to login again) and reduced resolution and graphics; who says there's no such thing as free lunch.
If we want high end graphics for the most recent titles we should expect a pricepoint of about 10-20$ a month, the graphics card alone of such a system might cost somewhere between 500-1000$ for the investment to be worth it, we would at the very least need to perform at that level for 25 months before replacing, that's not even considering the rest of the hardware. Low consumption users might find it differently, with a raspberry pi (rpi) 4b (less than 100$) or a simple core i3 SBC (about 250$ and up) can be enough to provide a cloud platform for everyday computing and some minor content creation. Leasing such an instance in the cloud would cost about 10-20$ monthly, and we can see how quickly our small investment pays off.

Developers can in many regards be low consumption users too, even a rpi 4b can host code-server that allows us to edit the code, that we then deploy to powerful cloud instances. If a powerful desktop would use 100h to train a neural network, it would be unavailable for the duration, but if we deploy to 100 equally strong nodes in the cloud we could pay at an hour increment and get the answer that quickly.
{: .notice--info}

To conclude the second post on automate me, we have seen that mobile and tablets have become powerful devices that together with cloud platforms have erased a lot of the initial differences between the platforms, desktop hybrid that allows mobile devices to use keyboards and mouse natively in a windowed experience draws us closer to a convergence, where desktops and mobiles are ubiquitous. By understanding our habits and how they interplay with our HCI needs we should be able to reduce the amount of devices we need, this saves us money, space, noise and even opens up to new possibilies. 

In the next section we continue down the ladder to smart devices and the internet of things, and how to use them and much more to create a context for automation and synergy.

When we lease cloud instances we might always want access to the IDE node, so keeping this as small as possible reduces costs when we are editing the code, we would usually create independent instances for running and testing.
{: .notice--info}


