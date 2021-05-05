---
title: "Automate me II: A flurry of devices"
excerpt_separator: "<!--more-->"
header:
  image: /assets/images/flurry_header.jpg
  caption: "Photo credit: [**Unsplash**](https://unsplash.com/@ranasawalha)"
categories:
  - automate me
tags:
  - Ubiquitous-Computing
  - Smart devcies
  - Cloud computing
  - Human Computer Interface
---
In 2020 every person world wide has on average 6 internet connected things with a total of nearly [30 Billion devices total](https://www.statista.com/statistics/802690/worldwide-connected-devices-by-access-technology/), it is truly a flurry of computers, and devices. From fitness trackers to server farms, understanding our habits and how it reflects our computational resource needs can both save us money as well as provide new features and remove the need for users attention in daily tasks.
<!--more-->

At the base of all our computational interactions we have everyday computing, with over [3.5 Billion people with smartphones worldwide](https://www.bankmycell.com/blog/how-many-phones-are-in-the-world), we see that this has been growing quickly over the last years, online presence, social media, news and storing our important files are all integer parts of our modern lifestyles, no matter where we are on the planet, with services like LinkedIn, online banking and emergency hotlines computation and internet have become utilities of necessity.

{% include figure image_path="/assets/images/automation2.jpg" alt="a home-assistant dashboard" caption="Robotics and autonomous systems are capable of doing complex tasks that has often been reserved for humans, now they can not only beat Kasparov in a digital version of chess, it could play him on a physical board as we would." %}

Most of our interactions with computation are clients to servers, depending on the task they distribute the workload differently, editing a local document needs no server interaction, while automations such as travel itiniraries are computed remotely. You can keep reading on how to build or extend your own cloud services [here](/automateme/), or additional information on personal devices [here](/workflow/desktop-hybrids/).

__*"If the brains behind automations are in the cloud, then IoT becomes its central nervous system."*__
{: .text-center}

Ubicomp is about so much more than just interacting with the data we ask for on the devices we're using, it is equally much about leveraging a context to provide automations that either removes or reduces the need for user attention. Lets imagine the use case of scheduling our robot vacuum, we could usually use a proprietary app to start or stop a cleaning cycle, or even make a schedule, for people with strict routines this could be enough. 

I have a more flexible day to day routine, and during the pandemic my trips out the door are fewer, so it would be nice if it knew when I wasn't home, or left the neighbourhood, to do this we need to provide a _presence_ context.

{% include figure image_path="/assets/images/dog_home.jpg" alt="a home-assistant dashboard" caption="It might not always be phone users, or even humans at home that makes us consider it not empty." %}

One simple way for home automation would be phone gps or home wifi, but for public spaces or guest users we cannot use these tools; it would be nice if they were general to their physical location, rather than related to a specific user. This is true for a lot of uses, from medical instruments to weather stations, in some cases such as storage facilites, factories etc might be nearly autonomous and need very little human oversight.

Amazon even has an automated [concept store](https://www.amazon.com/b?ie=UTF8&node=16008589011) that removed cashiers and registers, and rather used object and facial recognition to register your purchases.
{: .notice--info}

In fact, while we might not think of it, most of 'our' devices are not in our homes or office, they are represented as the enourmous and numerous server farms of cloud platform providers, from something as simple as file-syncing between devices and backups, to simulating economic models. Or the sheer scale of enterprise IoT in storage facilites and other automations, what we personally own is really just pees anyway, but there are a lot more of us potential IoT device owners out there, so it faces us with some grand challanges in protocol discovery, network topology and security. 

{% include figure image_path="/assets/images/connected_city.jpg" alt="a home-assistant dashboard" caption="Systems can grow incredibly large, from individual homes, to neighbourhoods and cities that mix private and public services." %}


Distribution also has another advantage, imagine our personal computer would use 10 hours on a problem, it would be unavailable for that duration, it might not be something we'd like to do with our laptops or phones, at least not without a charger. Some problems are much larger, like training deep neural networks, and would take even a high end stationary computer days if not weeks to train, this is where using commercial clouds becomes a game changer.

Renting a node equal to our personal computer, but paying on minute increments we could theoretically inflate to 36.000 instances for one minute (given that our problem can be solved in paralell). This ability to produce results and test our models quickly is essential, like sequencing a virus DNA and simulating vaccines to respond to a crisis. Just check out [colab](https://colab.research.google.com/notebooks/intro.ipynb) for how to use free GPU and TPU resources in the cloud.

{% include figure image_path="/assets/images/clustered.jpg" alt="a home-assistant dashboard" caption="These produce a lot of heat and noise, besides being a big investment, it also requires more maintenance, unless we need all of the power continuously, we might as well split the bill." %}

While the distinction can be a bit blurry in terms of which devices or 'things' are included as IoT, one distinction is to say it needs to be a network connected microcontroller, but this excludes small systems on a chip like [rpi zero](https://www.raspberrypi.org/products/raspberry-pi-zero-w/?resellerType=home) that has supports desktop OS like raspbian. Both of these groups of devices has sensors, actuators and limited amounts of local computational resource, but we usually need a server that can organize and execute heavier tasks.

{% include figure image_path="/assets/images/iot.jpg" alt="a home-assistant dashboard" caption="If you have a light with a motion detector, it might be reasonable to have both the light and sensor connected to the same controller, which locally manages to turn on the light when motion is detected, and works even without a server." %}

Distributed computing introduces two new factors to consider, network bandwidth and latency, how many packages of data can we send at once, and how quickly do we get a response once a request is made. Cloud gaming (or remotely operated robotics) are prime examples, the more sensitive our task is to small delays to our reaction time cloud computing might not always be our best bet.

On my local network I achieve about 10-15ms with only the client over wifi (AC/AX) using [parsec](https://parsecgaming.com/) on a Windows host, from commercial solutions lice [GeForce Now](https://www.nvidia.com/en-us/geforce-now/) I have about 20-50ms delay depending on which network I was connected to (office, cafe or home), you can even game with a free-tier on GeForce with lower graphics and resolution; now who says there's no such thing as a free lunch.

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="Some environments like VR are very sensitive to latency changes, and can cause nausea and other feelings of discomfort." %}

High end graphics on recent titles is about 10-30$ a month for commercial cloud gaming platforms, the graphics card alone of such a system might cost somewhere between 500-1000$ depending on our graphical setting and resolution. For a 500$ card to cheaper over time than the 10$ subscription it would need to provide the same level of quality on new titles up to 50 months (little over 4 years).

It is a different story for low and midt tier general purpose computers as a raspberry pi (rpi) (50-100$) or a core i3 build (+-250$), it is enough for most tasks and comes at a much lower initial investment making it accessible to people on low budgets. Leasing such an instance in the cloud would cost about 5-20$ monthly, and for most home server tasks this is ample power.

There are some considerations to the safety and availability infrastructure that commercial solutions otheriwse provide, take a look at the [infrastructure documentation](https://ceiku.github.io/automateme/infrastructure/) for more.
{: .notice--info}

{% include figure image_path="/assets/images/smarthome.jpg" alt="a home-assistant dashboard" caption="For end consumers IoT is really about smart homes and gadgets, it encompasses everything from the fitness data on their watch, to the grocery list written on the fridge, these devices, features and compromises makes individual solutions unique." %}

And to conclude the second post in the Automate Me series we should have noted that how devices let us peform our computational interactions have become more critical than the resources they provide locally, with good network bandwidth and low delay times the resources we need are at our disposal, anywhere. We should be aware of how to balance scaling up and out, some tasks require high responsivity and might set a lower bound on local resources, scaling up can let us solve complex tasks in very short timeframes.

In the next, and last post of the series we look closer at automations, how proprietary and open source differ in terms of features and required domain knowledge.

