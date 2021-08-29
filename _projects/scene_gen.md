---
title: "PhD Project: Scene Generation"
subtitle: Capturing distributions over environments to help robots and their designers understand the challenges they'll face.
layout: page
hide_hero: true
show_sidebar: false
card_image: assets/icra_2020.png
card_image_alt: Project image.
date: 20210829
usemathjax: true
---
<center>
<h1>{{page.title}}</h1>
<h5>{{page.subtitle}}</h5>
<h5><a href="https://github.com/gizatt/spatial_scene_grammars">github.com/gizatt/spatial_scene_grammars</a> [WIP!]</h5>
<img src="{{site.baseurl}}/assets/phd/demo_rooms.gif" alt="Gif of diverse kitchens being generated" border="10" />
</center>

My PhD project focuses on figuring out the tooling to capture a probability distribution $$p(world)$$ of real-world environments. Capturing a distribution over worlds is, at its core, a hard problem because it involves capturing a distribution over a mixed discrete and continuous distribution: specifically, how many objects of a given type are in a scene, and where those objects are, covary with each other in complex ways. If we could capture this distribution, we could:

1) Sample from $$p(world)$$ to generate tons of diverse, realistic, interesting environments to thoroughly test our perception and control algorithms in simulation (or for making game environments, or for quickly generating realistic backdrops in movies, etc...)

2) Use $$p(world)$$ as an outlier detector: when a robot encounters a new world $$world_{new}$$, evaluate the density $$p(world_{new})$$. If that density is abnormally low, then it knows it wasn't trained on worlds like this (and it should be wary!). The tools I use can even tell you what *part* of the world is surprising.

# Approach and aims

The above problem is almost absurdly broad; I'm exploring one of many possible avenues for tackling this problem. Specifically, I'm looking at using *scene grammars* as a representation for this distribution over worlds.

*Scene grammars* are a form of procedural model that supposes that 