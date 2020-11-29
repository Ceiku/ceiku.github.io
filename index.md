---
# You don't need to edit this file, it's empty on purpose.
# Edit theme's home layout instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
layout: home
author_profile: true
intro:
  - excerpt: 'From my days as an undergrad and tech enthusiast I started out with home automation and machine learning, it has been a long and interesting road and here are some of my projects along with some argumentation for design choices and architecture. I have tried to present the blog in layman term, the same way I have had to explain it to friends, family and students.'
feature_row:
  - image_path: /assets/images/vr_1.jpg
    alt: "Era of Calm Computing"
    title: "Era of Calm Computing"
    excerpt: "In this exploration of ubiquity in modern computing we will see how we can both save money, and gain new features as well"
  - image_path: /assets/images/scifi-ar.jpg
    alt: "Automate me"
    title: "Owning Our Services"
    excerpt: "Taking control of our own services is much more than replacing what we have, it is about getting what we want."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--inverse"
  - image_path: /assets/images/vr_1.jpg
    title: "VirtuPose"
    excerpt: "Borne from my graduating thesis, VirtuPose is the next platform for flexible and cheap pose recognition in VR"
---
{% include feature_row id="intro" type="center"%}

{% include feature_row %}

{{ site.description }}
