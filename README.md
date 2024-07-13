# HaloCage
A safety device that adds more protection to the existing Halo used in open-wheel racing
  
## Summary<a id='summary'></a>
The HaloCage is a design concept built around the existing Halo crash-protection system used in open-wheel racing series such as Formula 1.  

While the Halo itself does an excellent job of protecting the driver from being struck by larger objects, or in situations when the car is flipped over, it is not effective in shielding the driver from smaller objects and debris, which can also be very dangerous. The IndyCar series uses an aeroscreen for this reason, but remains the only series to do so. 

The HaloCage is meant to increase the level of safety that the Halo provides, while avoiding some of the tradeoffs and challenges that come with the Aeroscreen. Still in its early stages, the current design concept is a transparent 3D-printed honeycomb structure made from polycarbonate.  

The ultimate goal of this open-source project is to address and reduce some of the persistent hazards inherent to open-cockpit race cars, irrespective of the success of the HaloCage concept.
    
## Table of contents
[Summary](#summary)<br/>
  
[Background](#background)<br/>
&nbsp;&nbsp;[About the existing Halo device and its limitations](#about-the-existing-halo-device-and-its-limitations)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;[Key Features](#key-features)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;[Purpose](#purpose)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;[Limitations and incidents](#limitations-and-incidents)<br/>
&nbsp;&nbsp;[About the Aeroscreen](#about-the-aeroscreen)<br/>
  
[The HaloCage](#the-halocage)<br/>
&nbsp;&nbsp;[Requirements](#requirements)<br/>
&nbsp;&nbsp;[Design](#design)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;[Current state](#current-state)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;[In development](#in-development)<br/>
&nbsp;&nbsp;[Manufacturing and material considerations](#manufacturing-and-material-considerations)<br/>
&nbsp;&nbsp;[Testing and development](#testing-and-development)<br/>
&nbsp;&nbsp;[Challenges, concerns, and alternatives](#challenges-concerns-and-alternatives)<br/>
  
[Contributing](#contributing)<br/>
[License](#license)<br/>
[Sources and credits](#sources-and-credits)<br/>
  
## Background<a id='background'></a>
### About the existing Halo device and its limitations<a id='about-the-existing-halo-device-and-its-limitations'></a>
The Halo is a driver crash protection system used in open-wheel racing series, including Formula 1, Formula 2, Formula 3, Formula E, and others. It was introduced by the Fédération Internationale de l'Automobile (FIA) to enhance driver safety. The device consists of a curved bar placed above the driver's head, attached at three points to the vehicle's chassis.
  
The Halo has been credited with potentially having saved several drivers’ lives, or at least protecting them from severe injury.
  
#### Key Features<a id='key-features'></a>
* _Material_: Made from titanium, which provides a high strength-to-weight ratio.
* _Design_: The design includes a central strut in front of the driver’s helmet and two side struts, forming a protective 'halo' around the cockpit.
  
#### Purpose<a id='purpose'></a>
* _Protects against debris_: Designed to deflect large debris and prevent it from hitting the driver's head.
* _Supports vehicle structure_: In case of a rollover, the Halo helps to protect the driver by maintaining the structural integrity of the cockpit.
  
#### Limitations and incidents<a id='limitations-and-incidents'></a>
* _Partial protection_: While effective against large objects and preventing major injuries in crashes, the Halo has limitations in protecting against smaller debris or objects entering the cockpit.
* _Notable incidents_
    * In 2009, Felipe Massa was struck by a suspension spring from another car during qualifying for the Hungarian Grand Prix, resulting in serious head injuries. Although this incident occurred before the Halo's introduction, it could be argued that the large opening of the Halo might not have prevented such an incident, and it highlights the potential for small objects to cause significant injuries.
    * During the 2018 Russian Grand Prix, Pierre Gasly’s visor was struck by debris from another car due to a collision ahead. Fortunately, the visor held up, but the incident underscored the limitations of the Halo in protecting drivers from smaller debris​.
  
### About the Aeroscreen<a id='about-the-aeroscreen'></a>
An alternative to the Halo system is a transparent screen which was adapted in 2019 for use in IndyCar by utilizing the Halo as a structural frame.
  
Sebastian Vettel had previously tested a similar transparent screen called “Shield” in a Formula 1 car in 2017, where he reportedly completed one lap but stopped early due to distorted and blurred vision. Consequently, this design was never adopted for F1.
  
It remains unclear if or when the other series will implement a similar solution. This is where the HaloCage comes in.
  
It seems that the Halo device is here to stay in all “formula” racing categories, and it remains unclear if or when  is introduced, the need for a solution like the HaloCage remains.

The IndyCar series uses an aeroscreen for this reason, but remains the only series to do so, apparently due to a number of tradeoffs that other open-wheel racing series haven't been able to overcome.
  
## The HaloCage
### Requirements<a id='requirements'></a>
The goal of the HaloCage is to provide the highest level of protection for the drivers while having the least amount of impact on the car performance and the driving experience.
  
The following requirements will become more specific and quantifiable as development progresses:
  
* _Effects on visibility_
    * The HaloCage should be barely noticeable from the driver’s view.
    * Avoid any refractions, reflections, or other optical disturbances caused by the HaloCage.
    * Ideally, objects shouldn’t get stuck on the HaloCage, although this could be considered an acceptable tradeoff.
    * The visibility of the mirrors should not be impacted.
  
* _Effects on aerodynamics_
    * Excessive disturbances to the airflow should be avoided since this could impact the car’s performance.
    * Aerodynamic drag must be minimized.
    * Any aerodynamic forces that might cause the HaloCage to deform or come loose must be minimized or accounted for.
  
* The HaloCage should be as _lightweight_ as possible.
  
* Excessive _airflow-generated noise_ must be avoided.
  
* The HaloCage should not _get in the way_ when exiting the cockpit or removing the headrest, as is the case in F1.
  
* The HaloCage should not _become a hazard_, say if one of the sides of the HaloCage was somehow pressed in towards the cockpit due to a collision, or when sharp edges or pointy corners are created from damage.
  
* It should not negatively affect the _Halo itself_ in any way, for example:
    * If it required major design changes to the Halo
    * If it adversely affected testing or lead times for production
    * If it somehow diminished the safety that the Halo provides on its own
  
* _Manufacturability_: Producing a HaloCage should not be excessively expensive, complicated, or take too long.
  
* The HaloCage should be relatively _easy to install_ on top of the Halo.
  
* Ideally, _no fasteners or permanent bonding_ are needed and something like a set of latches would be enough to secure the HaloCage.
  
* Since the bodywork around the cockpit and below the Halo differs between cars, this might require a universal base design of the HaloCage, along with a custom portion that fills the gap between the base and the chassis.
  
### Design<a id='design'></a>
The current conceptual design is being developed in the computer-aided design software Autodesk Fusion 360. It is built around a publicly available [CAD file of the F1 Halo](https://grabcad.com/library/f1-halo-1).
  
#### Current state<a id='current-state'></a>
* Transparent, thin-walled honeycomb structure (less than 1mm or ~⅜”) covering most of the unprotected area susceptible to airborne objects and debris
* The depth of the walls is based on the direction of the airflow and the driver’s view: more depth towards the middle portion of the Halo, less depth towards the sides.
* The current honeycomb geometry should prevent objects that are 40mm (~1.5”) or larger from passing through.
* There are openings at the top allowing the drivers to place their hands on the Halo to help them get out of the cockpit.
  
#### In development<a id='in-development'></a>
* Contact areas between the HaloCage, the Halo, and the car body
* Mounting mechanism for easy installation and removal
* Connecting bridge that joins both halves of the HaloCage, which are currently divided by the Halo’s strut
* Structural reinforcements along the perimeter of the HaloCage
  
### Manufacturing and material considerations<a id='manufacturing-and-material-considerations'></a>
The transparent honeycomb structure could be achieved with 3d-printed polycarbonate, a lightweight and impact-resistant plastic used in applications such as bulletproof glass, astronaut helmets, and indeed the aeroscreen used in IndyCar.
  
However, due to the size limitations of 3D printers, the design will likely need to be broken up into multiple sections, some of which could be interlocking and fused or glued together.
  
### Testing and development<a id='testing-and-development'></a>
Simplified testing should suffice for the early stages to evaluate the design. Although helpful, It may not be necessary to create a replica model of the Halo, and the HaloCage could be tested on its own to get a ballpark estimate of its structural integrity.
  
Later on, small-scale prototypes could aid in assessing its aerodynamic effects and provide more data on its impact resistance.
  
Including the 3D model in a virtual racing simulator could give an idea of how the HaloCage affects visibility inside the cockpit.
  
Simulation tools such as computational fluid dynamics could further refine the design. Any advanced testing and development such as wind tunnel work is beyond the scope of this project and would have to be done by a professional team or a governing body such as the FIA.
  
### Challenges, concerns, and alternatives<a id='challenges-concerns-and-alternatives'></a>  
Meeting all requirements is a difficult task. The visibility and the aesthetics of the HaloCage are a major concern and could likely lead to rejection among the key people who need to develop and approve it. Moreover, the full potential of other crucial attributes like the design’s structural integrity remains to be seen.
  
Despite these challenges and concerns, innovation in this area is worthwhile. Even if the HaloCage concept ultimately doesn’t succeed, hopefully it will at least give rise to new ideas or solutions that could meet the unique safety demands in open-cockpit motorsports.
  
## Contributing<a id='contributing'></a>
At this stage, there is no collaboration yet. However, contributors are encouraged to independently improve upon the HaloCage concept, or come up with altogether different designs. Any contributions or ideas can be shared in the Discussions section.
   
## License<a id='license'></a>
This project is licensed under the MIT license, which is meant to provide maximum freedom of use. See the [LICENSE](https://github.com/c44w/HaloCage/blob/main/LICENSE) file for details.
  
## Sources and credits<a id='sources-and-credits'></a>
‘F1 Halo’ CAD file by Bhargav Gurrala on GrabCAD  
[https://grabcad.com/library/f1-halo-1](https://www.google.com/url?q=https://grabcad.com/library/f1-halo-1&sa=D&source=editors&ust=1720730265315240&usg=AOvVaw1OE-oDVbUqhmwqbVhZIqIU)  
  
IndyCar Aeroscreen  
Racecar engineering article
[https://www.indycar.com/news/2024/04/04-16-new-aeroscreen](https://www.indycar.com/news/2024/04/04-16-new-aeroscreen)  
  
Halo safety device  
[https://en.wikipedia.org/wiki/Halo_(safety_device)](https://www.google.com/url?q=https://en.wikipedia.org/wiki/Halo_(safety_device)&sa=D&source=editors&ust=1720730265316073&usg=AOvVaw1Vi41G8lp56olKWC9RynV6)  
[https://www.fia.com/news/how-make-f1-halo](https://www.google.com/url?q=https://www.fia.com/news/how-make-f1-halo&sa=D&source=editors&ust=1720730265316645&usg=AOvVaw1Aq6b2nZWpUATfcRciPD6L)  
  
Felipe Massa incident (pre-Halo)  
[https://www.theguardian.com/sport/2009/jul/25/felipe-massa-fernando-alonso-hungarian](https://www.google.com/url?q=https://www.theguardian.com/sport/2009/jul/25/felipe-massa-fernando-alonso-hungarian&sa=D&source=editors&ust=1720730265317383&usg=AOvVaw3BMKl_1NAY_JFJll_SuMQ_)  
[https://www.autoblog.com/2009/07/26/felipe-massas-skull-fractured-by-track-debris-during-hungarian/](https://www.google.com/url?q=https://www.autoblog.com/2009/07/26/felipe-massas-skull-fractured-by-track-debris-during-hungarian/&sa=D&source=editors&ust=1720730265318081&usg=AOvVaw3TE9VxOn7A8LENB4Zg5AGf)  
  
Pierre Gasly incident (post-Halo)  
[https://www.cnn.com/2018/10/02/motorsport/pierre-gasly-formula-one-russian-grand-prix-debris-hits-helmet-spt-intl/index.html](https://www.google.com/url?q=https://www.cnn.com/2018/10/02/motorsport/pierre-gasly-formula-one-russian-grand-prix-debris-hits-helmet-spt-intl/index.html&sa=D&source=editors&ust=1720730265318870&usg=AOvVaw35GPZzU8nEj6i5mg2SAyIB)  
[https://www.formula1.com/en/latest/article/gasly-hails-strength-of-f1-helmet-after-debris-incident-in-russia.7GdiJZuAoMsUGUMKmGKYq0](https://www.google.com/url?q=https://www.formula1.com/en/latest/article/gasly-hails-strength-of-f1-helmet-after-debris-incident-in-russia.7GdiJZuAoMsUGUMKmGKYq0&sa=D&source=editors&ust=1720730265319535&usg=AOvVaw3ghJbNyiNVRI6KmcgA8K8Q)  
