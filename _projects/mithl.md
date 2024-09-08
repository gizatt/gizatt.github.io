---
title: MIT Hyperloop Team
subtitle: Flying MIT's Hyperloop pod in the 2017 SpaceX Hyperloop competition.
layout: page
hide_hero: true
show_sidebar: false
card_image: assets/mithl.jpeg
card_image_alt: Project image.
date: 20170101
---
<center>
<h1>{{page.title}}</h1>
<h5>{{page.subtitle}}</h5>
<img src="{{site.baseurl}}/assets/mithl.jpeg" alt="MIT hyperloop pod" style="height: 300px;"/>
<img src="{{site.baseurl}}/assets/hyperloop_team.jpg" alt="MIT hyperloop team around pod" style="height: 300px;"/>
</center>

I had the great opportunity to be the software lead for MIT's Hyperloop Team around 2016-2017. The team was composed of a huge number of (mostly graduate) students from MIT AeroAstro, MechE, EECS, Sloan, and probably a bit more besides. I learned a ton about making a mechanically complex, multidisciplinary project *work* from these many talented folks.

Our design goal was to build a rail-riding, passive maglev transportation pod that could fly in a vacuum tube. Here's onboard video of our test flight, in which you can see (if you watch the wheel) that it does indeed **fly.**

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/U12rGwQfNb4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

---

<center><h2>Details</h2></center>
Our design goal was to build a passively-magnetically-levitated transportation pod compatible with a mile-long rail inside a mile-long vacuum chamber outside of SpaceX's headquarters in Hawthorne, CA, and to have it autonomously fly from one end of the track to the other as fast as possible. The project wound up involving immensely complex maglev, aero, and suspension design that put our huge team to work. But that hidden word "autonomously" gave me personally a pile of trouble; see our design report, linked below, for a look at the details of how we made it all work out.

Due to the team's hard work, our pod design -- which relied on passive magnetic levitation, fail-closed noncontact magnetic brakes, passive suspension, and uncertainty-aware inside-out state estimation won the first-round Design Competition. We worked hard to make the pod a reality, and after an arduous week certifying our pod's safety to SpaceX, were one of the just *three* teams (of ~30!) to get to fly at the final competition.

The video above is from a GoPro under the front of our pod from our run, embedded into my flight monitoring and control GUI. While we weren't allowed to fly at our design speed of ~250mph (no one was allowed to do so that year for reasons outside our control), we demonstrated that our vehicle was safe and stable at 60mph (still pretty fast!). The data (from O(50) sensors total) verified our design, lined up with our sims, and was generally a huge success.

---

<center><h2>Media Coverage</h2></center>
For stories about the team, check out some media coverage we got:
- [MIT News](https://news.mit.edu/2017/safe-at-any-speed-mit-hyperloop-0214)
- [Tech Review](https://www.technologyreview.com/2016/10/18/156745/the-hyperloop-pod-squad/)

---

<center><h2>Report and Code</h2></center>

- The team put together an [in-depth design report]({{site.baseurl}}/assets/MITHyperloop_FinalReport_2017_public.pdf) covering all aspects of our design.
- The core software is available at [github.com/MITHyperloopTeam/software_core](https://github.com/MITHyperloopTeam/software_core).
