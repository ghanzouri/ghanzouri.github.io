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

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig1.jpg)
{: refdef}
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

$$ \Delta L = \alpha*\Delta T * L_0 $$

$$L_0$$ : length found on the drawing
$$ \Delta L $$ : length difference before and after shrinkage
$$ \alpha = 2.3 * 10^{-5} K^{-1} $$ : linear shrinkage coefficient
$$ \Delta T $$ : temperature difference between melting and ambiant temperature

The ratio $$\frac{\Delta L}{L_0}$$ is thus constant and gives us the ratio scale to apply to the model of the part. By taking $$T_{melting} = 800°C$$ and $$T_{amb} = 20°C$$, we get $$\frac{\Delta L}{L_0} = 1.8 %$$. This report gives us the factor to add on each dimension of the digital part. We have therefore added a factor 1.018 to all dimensions to take account of shrinkage.

Second, we had to take into account the extra thicknesses to be added to the functional surfaces which are therefore provided for machining, so we also added during our calculations a 3 mm allowance on all the surfaces that will be machined (figure 2).

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig2.jpg)
{: refdef}
<center> Fig. 2: CATIA modelisation of the crapaudine </center>

### ii. Casting and stratoconception

We then export our CATIA model to Strato Pro (figure 3). This software will allow us to supervise the cutting of our model on a polystyrene plate. We can then stick with fusible glue. The polystyrene used is PSE (expanded polystyrene) which has properties superior to basic polystyrenes. So we define the tool, the arrangement of the different slices of the part on the plate, and the cutting pitch (here 0.4mm) which defines in how many slices the part will be divided.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig3.jpg)
{: refdef}
<center> Fig. 3: Strato Pro interface </center>

The information is then sent to the machine (figure 4) which immobilizes the plate thanks to a suction system (so no annoying jaws when cutting) to cut the part with the chosen tool. The model is finally assembled by hand (figure 5).

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig4.jpg)
{: refdef}
<center> Fig. 4: Stratoconception machine Charlybot </center>

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig5.jpg)
{: refdef}
<center> Fig. 5: Model assembly </center>

Machining time: 27 minutes

*Casting steps:*
For the preparation for the casting, we assemble a polystyrene pouring channel to the part which we will detach later.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig6.jpg)
{: refdef}
<center> Fig. 6: Polystyrene pattern with its downspout and funnel </center>

*Fabrication steps:*
* The part is immersed in a tank which is filled with sand without binder, then the tank is vibrated, which has the effect of filling all the interstices and cavities of the polystyrene model, as if it were a 'liquid.
* A metallic mass is placed on the upper part of the sand to maintain a certain pressure throughout.
* We pour the aluminum alloy AlSi13 at 800 ° C on the polystyrene
* The polystyrene sublimates and the alloy takes the place of polystyrene
* Cooling phase then the tank is inverted (= stall phase)
* Deburring phase: we remove the bunch / runner with a saw and we obtain the part

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig7.jpg)
{: refdef}
<center> Fig. 7: Filling the metal container on the vibrating platform </center>

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig8.jpg)
{: refdef}
<center> Fig. 8: Cutting of the downspout </center>

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig9.jpg)
{: refdef}
<center> Fig. 9: Final piece obtained in Lost Foam </center>

## b. Sand casting

However, we did not use our piece obtained by Lost Foam. Indeed, even if we had chosen to realize it by this molding process, it turned out in practice that the use of the model by this process posed many problems if we really wanted to respect the conditions of the definition drawing of the toad. This is why we chose to produce the part in sand molding for the rest of the project.

The first problem we encountered with the Lost Foam process was the quality of the material we had to use to make the model. Indeed, the material once passed on the stratoconception machine gave the model a very bad surface condition. Much worse than the wooden model for the sand casting process. In addition, when we converted the CATIA file into a file compatible for the stratoconception machine, we were asked to enter the software that we just wanted to use the simplex mode but not the duplex mode. This choice had some consequences on the realization of the model in the stratoconception machine. Furthermore, the final model did not totally resemble the CATIA file that we had produced. For example, the entire lower internal part of the basket was not made by the machine or rather was incomplete.

*Mold making:*

We start to prepare the lower frame by placing the lower part of the pan flat on the table, the frame must then be filled with sieved sand, packing well on the piece and on the edges being careful not to move the model (figure 10). We can then fill the rest of the chassis by scraping at the end to obtain a flat surface.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig10.jpg)
{: refdef}
<center> Fig. 10: Wood crapaudine pattern </center>

We put talcum on top to prevent the sand from the upper chassis sticking to the sand from the lower chassis (figure 11), with four washers at the four corners of the lower chassis. So, when we add the sand from the upper part, the joint plane will be perfectly consistent.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig11.jpg)
{: refdef}
<center> Fig. 11: Chassis with talc </center>

We turn the frame over to place the upper frame on the four washers, then we place the upper part of the model on the other already placed part of the lower model, paying attention to the positioning, in the same way we fill with the sifted sand to the upper part of the chassis by compacting it gently.

**Demoulding:** The two parts of the model are removed with an appropriate screw without altering the imprint of the model already made.
**Core:** We place the core in the right place in the impression (figure 12), then we start to realize the casting system.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig12.jpg)
{: refdef}
<center> Fig. 12: Core placed in the cavity </center>

**Pouring system:** The pouring descent is created using a hollow tube. We create the longest possible attack with a constant section. The pouring funnel is created to have an opening large enough to facilitate pouring.

**Rewinding:** The upper chassis is replaced on the lower chassis.

**After casting:** After preparing the aluminum, we start to cast aluminum.

**Stall:** After having left a little cooling time, we break the mold to recover the bunch

**Clearing:** We break the core with a hammer and chisel

**Deburring:** The casting system is removed.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig13.jpg)
{: refdef}
<center> Fig. 13: Alloy casting AlSi13 Aluminium </center>

## c. Comparison of the two processes

*Sand casting*
***Advantages***: No toxic vapor, stronger ferrous alloy, model reusable many times, low cost, sufficient cohesion and refractoriness
***Disadvantages***: Study of the necessary molding, limited complexity, destructible mold

*Lost foam casting*
***Advantages***: No joint plane, no demolding operation, sand without binder (recycling, better precision and surface condition), no hard core to introduce, undercut possible
***Disadvantages***: Toxic vapor, unable to reuse the model, final part with a poor quality surface finish

# III- Final part machining

After molding in sand casting, we got our final part. To be able to respect the different tolerances and dimensions, it is necessary to machine the part. The surfaces to be machined are shown in red in the photo below:

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig14.jpg)
{: refdef}
<center> Fig. 14: Functional surfaces </center>

We cut this part into two phases. The first consists in machining the part in *lathing*, then in *milling*. Indeed, it would have been possible to carry out these two phases on the 3-axis milling center. However, the isostatic assembly takes a long time to set up when we have to change the position of the part: we need to turn it once. We therefore take advantage of the geometry of revolution of the part to prefer to start with a turning phase with the aim of gaining productivity. We have the following machining ranges:

## a. Manufacturing tasks

### i. Lathe

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig15.jpg)
{: refdef}
<center> Fig. 15: Lathing sequences </center>

### ii. Milling

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig16.jpg)
{: refdef}
<center> Fig. 16: Milling sequences </center>

## b. Machine settings and parts positioning

### i. Lathe
We therefore place the blank in the workpiece chuck.
The positioning is done by internal jaws at the level of surface A in order to be able to cart surface D. (figure 17). We choose the cutting parameters using the formula $$ \frac{1000*V_c}{\pi D} $$ and adjust the turn (figure 18). We start with a roughing phase and then a finishing phase.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig17.jpg)
{: refdef}
<center> Fig. 17: Positioning of the part on the lathe </center>

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig18.jpg)
{: refdef}
<center> Fig. 18: Lathe setting </center>

### ii. Milling

The first step is to put the part in position isostatically as follows:

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig19.jpg)
{: refdef}
{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig20.jpg)
{: refdef}
<center> Fig. 19, 20: Isostatic mounting on the CNC machine </center>

Three supports correspond to a flat support, 2 supports correspond to a linear support and finally a single support corresponds to a specific support (here realized thanks to a ball). These three types of supports are needed to achieve isostatic MiP. It is necessary to post these supports as much as possible on machined surfaces to have the best quality of support and therefore of machining possible.

## c. Verification

### i. Lathe
We choose the thickness of the pass. After each of its passes, we check with a caliper the diameter of the cylinder in order to ensure compliance with the quotes.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig21.jpg)
{: refdef}
<center> Fig. 21: Checking dimensions after each pass (Lathing) </center>

### ii. Milling

The dimensions are checked using a micrometer. Note that the dimensions of the holes have been reduced in order to be certain of respecting the dimensions imposed by the plan.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig22.jpg)
{: refdef}
<center> Fig. 22: Dimension verification (milling) </center>

# IV- Quality control of the final part

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig23.jpg)
{: refdef}
<center> Fig. 23: GD&T drawing specifications in red </center>

## a. Dimensions verification

We measured the different dimensions of the workpiece and compared them to the dimensions on the engineering drawing. We had a calliper and a 50mm size isomer available. We carried out the various measurements using calipers. However, the 50mm size isometer was defective, we could not measure the inside diameter of 50mm. All the values are listed in the following table:

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig24.jpg)
{: refdef}
<center> Fig. 24: Table of dimensional values </center>

The green boxes show that certain values were respected: belonging to the tolerance interval or a relative deviation <1%. However, most are wrong (red box) due to the foundry defect: *shrinkage*.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig25.jpg)
{: refdef}
<center> Fig. 25: Shrinkage defect </center>

## b. Surface condition

To check the surface condition of the inner cylinder, a unidirectional roughness meter equipped with a sensor was used. We have positioned the part (figure 26) and the roughness sensor moves at constant speed along the roughness profile (inner cylinder), variations in the height of the sensor are recorded and processed to display the roughness values.

We are particularly interested in the roughness Ra and Rt. The roughness Rt corresponds to the difference between the highest projection and the lowest trough of the profile. The roughness Ra corresponds to the arithmetic mean roughness of the profile. It is used as an overall assessment of the amplitude of the roughness of the profile but does not give any information on the spatial distribution of the irregularities of the profile nor of the shape of the profile. The following values are found:

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig26.jpg)
{: refdef}
<center> Fig. 26: Measured roughness </center>

On the part definition drawing, the required average roughness Ra is 0.8. For our part we obtained an average Ra of 0.81 which seems correct. However for Rt we found 10.232 on average (8 times larger than what is indicated on the drawing), this is related to the machining and the cutting tools used.

## c. Coordinate Measuring Machine (CMM)

The CMM machine (Coordinate Measuring Machine) makes it possible to compare one of the surfaces with reference plane surfaces in order to determine the dimensional deviations. This then makes it possible to determine whether the part conforms or not to the desired dimensioning derived from the plane of the crapaudine.

We used the CMM to check the constraints of cylindricity of surface A, and of flatness of surface C and the perpendicularity between surfaces A / C with the Metrosoft QUARTIS software. We have chosen to check these surfaces in view of the tolerances specified on the plan.

The CMM measurement method is done using a probe. To measure the various constraints, the machine palpates the surfaces to be characterized. Several scores are necessary for a good measurement. The number of points measured is a parameter that one chooses. The greater the number of scores, the closer we get to real surfaces. The software is based on the least squares method to best approach all the measured points. However, we had 30 minutes available on the CMM machine. Choosing a lot of points would take an enormous amount of time. So a compromise had to be found. We therefore chose to take 6 points per surface.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig27.jpg)
{: refdef}
<center> Fig. 27: CMM indicator </center>

**Implementation:**

To carry out the three-dimensional measurement of the basket, we started by calibrating the probe. Next, we started probing the different surfaces with which geometric specifications are associated. Once the coordinate system had been defined, it was possible, as described above, to measure the flatness and the cylindricity of the desired surfaces. We then carry out the various measurements in relation to reference surfaces which we specify in the software. The following results are obtained:

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig28.jpg)
{: refdef}
<center> Fig. 28: Results obtained after our study on CMM </center>

We therefore conclude that the flatness tolerance of the surfaces C is verified, while that concerning cylindricity A and perpendicularity are not respected. There is a relative difference of 689% and 999% difference between the measured value and the tolerance imposed on the drawing. This is mainly due to the fact that our part has foundry defects (figure 25), foundry bodies and expansion.

{:refdef: style="text-align: center;"}
![Yosh Ginsu]({{site.baseurl}}/assets/img/crapaudine/fig29.jpg)
{: refdef}
<center> Fig. 29: Ideal position for CMM study </center>

This would be the ideal position to carry out the full study with CMM. We decided to choose the first one (figure 27) for the sake of time on the machine.

# V- Conclusion

We have noticed that, on several points, our part did not respect the tolerances imposed by the plane of figure 1. The tolerances of cylindricity A and perpendicularity A / C are not verified by measurement on the CMM. We still check the flatness of plane C. Unfortunately, our part had foundry defects such as shrinkage (figure 25). Besides, the base plane has dimensional errors on non-machined surfaces. The verifications of the specifications were complicated (no area of references) to validate.
