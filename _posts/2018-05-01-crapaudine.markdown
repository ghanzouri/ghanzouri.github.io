---
layout: post
title:  Casting crapaudine manufacturing project
date:   2018-05-01 13:32:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: /crapaudine/crapaudine.jpg # Add image post (optional)
tags: [Manufacturing, Product Design, Catia, CAD, Lost Foam, Sand casting, CNC, Milling, Lathe, CMM]
author: Ilies Ghanzouri # Add name author (optional)
---

# Manufacturing project of the crapaudine
#### January 2018 – May 2018, Paris, France

# I- The project

The objective of this project was to follow all the stages of manufacturing of a part: starting from the engineering drawing, being able to produce a part to standards and controlled intended for sale. The piece we were given to follow is the crapaudine (figure 1). The crapaudine is a common piece in the industry that allows the rotation of a vertical shaft whose load is allong its axis.

![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig1.jpg)
<center> Fig. 1: Engineering drawing with GD&T specifications </center>

We adopt the following approach:
* Study the drawing of the crapaudine (geometric specification, etc.),
* Model in CATIA to create a model allowing us to melt the pattern,
* Machining the part using CNC machines
* and finally verify in metrology to check the concordance with the specifications and validate the project.
The piece will be made in Aluminium AlSi13.

# II- Casting

## a. Lost Foam Casting

To realise our piece, we first opt for the “Lost Foam” process. The principle of Lost Foam is to give the desired shape to polystyrene (PSE or PMMA). Then sand with binder around the polystyrene. Then, during casting, the polystyrene will evaporate in the form of gas under the temperature of the molten alloy.
We must therefore obtain a model of the polystyrene part to be able to use this process. This is why it is decided to manufacture this model ourselves in stratoconception.
For this, we will use the software “Strato Pro” of stratoconception machine. So we first need to model the crapaudine on a computer using CATIA software.

### i. CATIA modeling
When creating the CATIA model, it was necessary to take into account two factors modifying the dimensions of the definition drawing provided:
First, it was necessary to take into account the phenomenon of shrinkage of material which occurs during casting. This phenomenon is observed during the cooling of the alloy after solidification. The decrease in temperature results in a decrease in the volume of the alloy. This shrinkage is linear and can be expressed by the formula:
$$ f_x=2 $$
