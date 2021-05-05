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
It might have been hard to imagine at the dawn of personal computers in the 80's just how pervasive they would become today, with our myriad of personal smart gadgets and cloud services. And about 15 years prior to smartphones, place Mark Weiser laid forth a computer paradigm called [Ubiquitous computing](https://www.lri.fr/~mbl/Stanford/CS477/papers/Weiser-SciAm.pdf) (ubicomp), in this era of calm technology, the computers fade into the background.
It is a paradigm born from how we design human-computer interfaces (HCI), and the context it provides our computations, it should make the data we would want or require available comfortably, as we move between home, office, hobbies and vacations. 


<!--more-->

The first wave of computing came with huge mainframes, these large and expensive machines could occupy everything from a room to whole factory floors, very often we coded with no separation between the hardware and the user (the earlier versions was usually programmed with punching cards). These machines shrunk, became more efficient and for the same cost, by the 80s we entered the second wave of computing, the 'personal' computer.

{% include figure image_path="/assets/images/computation-at-work.jpg" alt="devices in work environments" %}

If we look past the relative change in size, they came with operating systems (OS) that in the beginning only provided simple commands and file management, developed over time to provide pointing interfaces such as the mouse and (touch) screens etc. These developments allowed computers to become personal, as we needed to know less about how the machinery work, the user interfaces (UI) is the same if we are browsing images of cats, creating special effects, or even simulating black holes.

Without getting too technincal, the only thing we need to learn about the two common [architectures for general-purpose computing](https://cs.stanford.edu/people/eroberts/courses/soco/projects/risc/risccisc/), RISC (ARM) and CISC (x86), is that generally they represent the mobile and desktop markets respectively. The ARM architecture has traditionally been popular in mobile devices due to its low power consumption, and was usually computationally weak devices, though a lot changed since the iconic iPhone:

| year |name|cpu|ram|display|storage|camera|
| 2007 | iphone 2G | 412mhz | 128mb | 3.5 inch 320x480 | 4-16gb | 1.92 mp |
| 2013 | HTC One | 1.7ghz quad-core | 2gb | 4.7 inch 1080x1920 | 32-64gb | 4mp
| 2020 | samsung  s20 ultra | 2ghz octa-core | 12gb | 6.9 inch 1440x3200 | 128-512gb | 108mp (array) |

Between these devices stand 13 years of inovation, it is a perfect example of moore's law at work, but that's not the whole reason why the power we could squize into our pockets just kept increasing. As updates kept coming [we kept bying](https://www.statista.com/statistics/263437/global-smartphone-sales-to-end-users-since-2007/) and the sales have increased tenfolds over this period, making it an equally big [market share](https://gs.statcounter.com/platform-market-share/desktop-mobile-tablet/worldwide/#monthly-200901-202010) as desktops. In fact, smartphones can now be compared in power to low and mid range laptops, the only difference between them seems to be HCI, the desktops provide keyboard and mouse support, with a windowed experience on one or more monitors that allows us to multitask or organize larger projects comfortably.

{% include figure image_path="/assets/images/ecosystem.jpg" alt="a home-assistant dashboard" caption="A creative workstation and devices in a very propietary homogenous ecosystem." %}

While the smartphones are a wonder device in terms of HCI that in many cases support these periphirals, there hasn't been large innitiative to create a mobile OS that provide the same windowed multitasking environment; until now, Samsung DeX and iPad OS is the first comfortable mobile-desktop hybrids. Microsoft has gone the other way with their Surface, which is desktop hardware shaped as a tablet, they have made some changes to Windows to make it touch interface friendly.

{% include figure image_path="/assets/images/samsungdex.PNG" alt="a home-assistant dashboard" caption="Samsung dex provides a rich windowed environment, even a lot of common keybindings etc are present. [credit](https://www.samsung.com/us/explore/dex/)" %}

The reason why we would hardly notice the switch (and tablet computing is trending) is that most of our tools and files now exist in the cloud, as end consumers we only need to store personal or sensitive data locally or encrypted. My work as a developer is done in cloud tools such as vs code remote or code-server, full IDE environments available as webviews, it's like having my work environment anywhere there's a browser. Mobile devices are also cheaper, and makes no noise compared to their laptop or stationary counterparts.

{% include figure image_path="/assets/images/office_with_view.jpg" alt="a home-assistant dashboard" caption="With a cellular tablet, anywhere can become your office, and a simple powerbank goes a long way to extend it to days." %}

It is not an unknown problem to become "plaform dependent" however, eg. Apple TimeMachine backup feature is available on macOS devices, where you can use any external storage to make backups of all your personal data incrimentally, it is easy to use and has a good interface; it is easy to understand that someone would keep bying the same platform. But it's only easy in so far as you keep bying from the same manufacturer, this even applies to new platforms (eg. smart watch to phone compatability, or software to OS).
These are proprietary walls to our ubuquitous dream, but some people just don't do that kind of compromise.

{% include figure image_path="/assets/images/automation.jpg" alt="a home-assistant dashboard" caption="The mess hidden under the 'rug' from navigating multiple ecosystems, which is what we will try to solve as best as possible in the coming posts." %}

To some people this lack of control may have led them to think "No way I would accept that" or "I could do better myself", this stubborn denial to compromise is what I think is the proud backbone of todays vibrant open source communities. In fact, one of the most successful open source projects started out from just that. Linus started in his "basement", creating the first Unix kernel, the basis for Linux OS that today is the most widely used OS in the world, from mobile devices to supercomputers. Some open source projects are funded and provide steady realible updates and features, but unlike most commercial solutions they require some configuration, in turn they provide equal if not more features than commercial solutions.

{% include figure image_path="/assets/images/ha_dash.png" alt="a home-assistant dashboard" caption="A simple Home-Assistant dashboard that unifies a lot of brands and services into one interface, from different brand lightings, to custome public transport departures and chores." %}

Perhaps we don't want to replace everything, no need to re-invent the wheel, and commercial solutions often offer a lot of contextual automation out of the box, using google as a mail provider creates an itinirary that tracks my journey when I recieve a flight confirmation etc into my inbox. It offers a calculated departure time from my residence based on traffic estimates, and now in the pandemic it even offers the most up to date regulations relevant for the trip. 

For most people, this convenience far outweighs the consequence of ones flight information being visible to google; it was to begin with anyway.
{: .notice--info}

What we cannot do here is ask Alexa or Siri to get this information for me just as easy, this is where open source solutions shine, they let us "jump" these proprietary walls to connect services and created features that companies cannot or will not do themselves. That is what the Automate Me project is for, the repository has a collection of open source services and tools from common infrastructure to home automation that works together seamlessly. 

The calm era of computing actually thrives when we give it some contextual data to work with, it stops having to ask or be told, as with the travel itinrary, it saves the user from spending any attention to the task. Out of sight and out of mind is a good way to think of what should make services and devices "smart", and paraphrasing Nicholas Negroponte from his [ted talk](https://www.ted.com/talks/nicholas_negroponte_a_30_year_history_of_the_future?language=en):

*"An oven is not smart because when I put a chicken in it, I can set the temperature and other dials from my phone, it would be smart if it ask how well cooked I'd like my chicken, perhaps already know."*
{: .text-center}

As we move forward through these posts we will see some major challenges, and how we might move our digital lives from dials, to become unseen and autonomous. The next post looks closer at our personal and other HCI devices, their history and how they have changed together with our computational habits, and if you are interested in getting more hands on to improve your project or get started, go straight to my [AutoLife documentation](https://ceiku.github.io/AutoLife/).
