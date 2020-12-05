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
In 2020 every person world wide has on average 6 things connected to the internet, it is truly a flurry of computers, and things. From fitness trackers to server farms, understanding our habits and how it reflects our computational resource needs can both save us money as well as provide new features and remove the need for users attention in daily tasks.
<!--more-->


{% include figure image_path="/assets/images/automation2.jpg" alt="a home-assistant dashboard" caption="Robotics and autonomous systems are capable of doing complex tasks that has often been reserved for humans, now they can not only beat Kasparov in a digital version of chess, it could play him on a board as we would." %}

At the base of all our computational interactions we have everyday computing, with over x% of the population online on a personal device, we see that this has been growing quickly over the last years, online presence, social media, news and storing our important files are all integer parts of our modern lifestyles, no matter where we are on the planet, with services like LinkedIn, online banking and emergency hotlines computation and internet have become utilities of necessity.

Most of our interactions with computation are clients to servers, depending on the task they distribute the workload differently, editing a local document needs no server interaction, while automations such as travel itiniraries are computed remotely. If you want to keep reading on how to build or extend your own cloud services, read on [here](/automateme/), additional information on personal devices [here](/workflow/desktop-hybrids/).

__*If the brains of automations are in the cloud, then IoT is the central nervous system.*__
{: .text-center}

Ubicomp is about so much more than just interacting with the data we ask for on the devices we're using, it is equally much about leveraging a context to provide automations that either removes or reduces the need for user attention. Lets imagine the use case of scheduling our robot vacuum, we could usually use a proprietary app to start or stop a cleaning cycle, or even make a schedule, for people with strict routines this could be enough. 

I have a more flexible day to day routine, and during the pandemic my trips out the door are fewer, so it would be nice if it knew when I wasn't home, or left the neighbourhood, to do this we need to provide a _presence_ context.

One simple way for home automation would be phone gps or home wifi, but for public spaces or guest users we cannot use these tools; it would be nice if they were general to their physical location, rather than related to a specific user. This is true for a lot of uses, from medical instruments to weather stations, in some cases such as storage facilites, factories etc might be nearly autonomous and need very little human oversight.

Amazon even had an automated concept store that removed cashiers and registers, and rather used object and facial recognition to register your purchases.
{: .notice--info}

In fact, while we might not think of it, most of 'our' devices are not in our homes or office, they are represented as the enourmous and numerous server farms of cloud platform providers, from something as simple as file-syncing between devices and backups, to simulating economic models. Or the sheer scale of enterprise IoT in storage facilites and other automations, what we personally own is really just pees anyway, but there are a lot more of us potential IoT device owners out there, so it faces us with some grand challanges in protocol discovery, network topology and security. 

If we imagine the top of the line desktop would use 10h to compute one problem, then any other interaction in between would add to the total duration, in other words it is unavailable. Since these machines could easily use hundreds of hours to train deep neural networks, having the ability to inflate, to scale our work to another powerful node, or distribute it over many; if we lease cloud instances at 1m intervals, then hundreds of hours can be reduced to a single minute. This ability to produce results and test this quickly is can be essential, like sequencing a virus DNA and simulating vaccines to respond to a crisis. Just check our colab for how to use free GPU and TPU resources in the cloud.

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="I don't know  about you, but I have never been fond of all the cables, the noise from disks and fans of using stationary computers, (hearing a gaming rig under load is like experiencing a plane perpetually take of besides you)." %}

While the distinction IoT can be a bit blurry in terms of which devices, or 'things' are included, one distinction is to say it needs to be a network connected microcontroller.
But this excludes small systems on a chip like rpi zero that has supports desktop OS like raspbian, and while both of these groups of devices has sensors, actuators and limited amounts of local computational resource, we usually need a server that can organize and execute heavier tasks.

If you have a light with a motion detector, it might be reasonable to have both the light and sensor connected to the same controller, which locally manages to turn on the light when motion is detected. This simple automation is easy to do with limited resources, and we avoid delayed action from requesting an answer remotely and most importantly the feature works even if the servers would be down.

{% include figure image_path="/assets/images/vr_common.jpg" alt="a home-assistant dashboard" caption="As we can see, the responsibilities of providing computational resources is not a black and white picture, this allows us to scale up and out to balance costs, uptime and responsivity" %}

Distributed computing introduces two new factors to consider, network bandwidth and latency, how many packages of data can we send at once, and how quickly do we get a response once a request is made. Cloud gaming (or remotely operated robotics) are prime examples, the more sensitive our task is to small delays to our reaction time cloud computing might not always be our best bet.

On my local network I achieve about 10-15ms with only the client over wifi (AC/AX) using parsec on a window host, from commercial solutions lice GeForce I have about 20-50ms depending on which network I was connected to (office, cafe or home), these are a small nuisance at best since you can even game with a free-tier on GeForce with lower graphics and resolution; now who says there's no such thing as a free lunch.

If we want high end graphics for the most recent titles we should expect a pricepoint of about 10-20$ a month, the graphics card alone of such a system might cost somewhere between 500-1000$ for the investment to be worth it, we would at the very least need to perform at that level for 25 months before replacing, that's not even considering the rest of the computer components. This changes as we move towards low tier computers such as raspberry pi (rpi) 4b (less than 100$) or a simple core i3 SBC (about 250$ and up) can be enough to provide a cloud platform for everyday computing to some minor content creation, the initial investment is also a lot lower.

Leasing such an instance in the cloud would cost about 5-20$ monthly, so investing in a local system can be cost efficient; but there are some considerations to the safety and availability infrastructure that commercial solutions otheriwse provide, take a look at the [infrastructure documentation](https://ceiku.github.io/automateme/infrastructure/) for more.

For end consumers IoT is really about smart homes and gadgets, it encompasses everything from the fitness data from their watch, to the list written on the fridge, the devices, features and compromises we make to get them are all different. So there is no two smarthomes quite the same, I have a in-ear headset that is most frequently in use when I work out, so a practical automation was to have my workout playlist start playing when they connected to my phone; great for me, maybe not for you. The major challenge is selecting good devices and software, in many cases this leads to high expenses, but stubborn and crafty people usually find a way (as getting a reluctant old roomba to be wi-fi connected.)

And to conclude the second post in the Automate Me series we should have noted that how devices let us peform our computational interactions have become more critical than the resources they provide locally, with good network bandwidth and low delay times the resources we need are at our disposal, anywhere. We should be aware of how to balance scaling up and out, some tasks require high responsivity and might set a lower bound on local resources, scaling up can let us solve complex tasks in very short timeframes. In the next and last post of the series we look closer at automations, how proprietary and open source differ in terms of features and required domain knowledge.

