---
layout: post
title:  UAV Package Delivery System
date:   2019-05-17 13:32:20 +0300
description: #You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: /dassault/post-1.jpg # Add image post (optional)
tags: [Product Design, Mechatronics, Catia, CAD, 3Dprinting]
author: Ilies Ghanzouri # Add name author (optional)
---

# Design of the package delivery system at Dassault UAV Challenge
#### September 2019 – May 2019, Paris , France

The Dassault UAV Challenge is an aerospace student competition dedicated to Unmanned Air Vehicle (UAV) domain. It was organized by Dassault Aviation. The challenge was based on the same hexacopter platform for each team (to be assembled with components provided by Dassault Aviation).

Each team had to design a home-made package delivery system and integrate it in the hexacopter. The main part of the development focused on the system integration, the real-time software development and flight tests. The challenge lasted 7 months to perform the whole development and a 2-days competition final in May with several tests and workshops had to be completed.

To perform the competition, each team had to design and integrate its own package delivery system in its hexacopter, including:
* a storage system to carry and release three packages on demand
* associated embedded algorithms to deliver autonomously and precisely each package on pre-defined target points

In our team, I was personally in charge in designing the package delivery system.

# I.	Package delivery system
## a.	Description of the delivery system

The system is composed in two parts.

The first one is a cylindrical compartment which will contain the 3 packages and 1 empty space. This cylinder rotates inside the external fixed cylinder by the means of a servomotor located at the base of the drone. This servo can rotate up to 270°.

On the other hand, this internal cylinder is guided in rotation by means of an external cylindrical base which is fixed to the drone. A cover attached to the outer cylinder is located at the base of the release system and has a door actioned by a servomotor.

When the camera detects a cross, the compartment (the inner cylinder) rotates and places the package corresponding to the colour of the cross above the door. Then the servomotor opens the door and drops the package on the cross.

![Yosh Ginsu]({{site.baseurl}}/assets/img/dassault/fig1.jpg)
<center> Fig. 1: External cylinder with servo slot that rotates the internal cylinder </center>

![Yosh Ginsu]({{site.baseurl}}/assets/img/dassault/fig2.jpg)
<center> Fig. 2: Cover for the external cylinder </center>

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/dassault/fig3.jpg)
{: refdef}
<center> Fig. 3: Internal cylinder </center>

## b.	Packages description

The packages are defined as follows:
*	Rectangular prism: height 80mm, base 30x30mm
*	3 colours: red, yellow, blue
*	Free choice of material (but homogeneous)
*	No weight constraint
*	No parachute



















a
