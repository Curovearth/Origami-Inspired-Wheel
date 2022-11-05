---
layout: default
title: Paper-1
parent: Research Papers
---


# Bio-inspired Tensegrity Soft Modular Robots
{: .no-toc}

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

## Metadata

- Title: Bio-inspired Tensegrity Soft Modular Robots
- URL: [https://arxiv.org/ftp/arxiv/papers/1703/1703.10139.pdf](https://arxiv.org/ftp/arxiv/papers/1703/1703.10139.pdf)
- D. Zappetti, S. Mintchev, J. Shintake, and D. Floreano | Laboratory of Intelligent Systems at Ecole Polytechnique Fédérale de Lausanne (EPFL),  H1015 Lausanne, Switzerland | davide.zappetti@epfl.ch

## Highlights & Notes

### Abstract
---
- In this paper, we introduce a design principle to develop novel soft modular robots based on tensegrity structures and inspired by the cytoskeleton of living cells.
- Tensegrity structures are lightweight, can undergo large deformations generated by internal or external forces, and can resist large compressive forces.
- Tensegrity in biological and robotic systems
- develop icosahedron tensegrity structures with programmable variable stiffness that can deform in a three-dimensional space.
- We also describe a method to add contraction movement by means of tendon-driven actuation and validate the approach in a proof-of-concept crawling, multi-modular worm
- inspiration by the mechanical structure of multicellular organisms cells
- We also describe a tendon-driven contraction mechanism to actively control the deformation of the tensegrity modules. Finally, we validate the approach in a modular locomotory worm as a proof of concept.
- However, every cell has a cytoskeleton, which is an extremely complex network made of two types of interconnected fibers [14]: rigid microtubules and bendable actin filaments (Fig. 1a). This architecture, which is responsible for the shape, stiffness, and strength of the cell can be formally described as a tensegrity struc- ture [15]


### Introduction
---
- The term “tensegrity” has been coined by architect R. Buckminster Fuller to describe a structure that maintains its mechanical integrity throughout the pre-stretching of some elements constantly in tension (called “cables” in red in Fig. 1b) connected in a network with other elements constantly under compression (called “struts”
- modular and swarm systems fall in two categories: systems made of complex units that can individually move or perform some tasks and systems made of simple units that can move or perform tasks only when they are assembled with other units.
- Yet another example of a tensegrity robot is SUPERball developed at NASA [20], which is able to roll, even on rough terrains, with an optimized control of the six embedded actuators
- morphofunctional properties emerge from the assembly of multiple units, as in biolog- ical multi-cellular organisms
- Tensegrity Structure Selection
- Different tensegrity structures can be obtained according to the number of struts and cables, the network configuration (e.g. struts and cables positions in the three-dimen- sional space), the cables’ stiffness and how much they are pre-stretched
- Three main criteria have been applied to select the main tensegrity structure for a modular tensegrity robot. The first criterion is that the main soft module should be able to deform (e.g. stretch or contract) in all directions to augment the morphological di- versity of the assembly and comply with objects and surfaces in a three-dimensional space. The second criterion is that the tensegrity structure should involve the smallest possible number of struts and cables to ease the manufacturing and assembling. The third criterion is to favor network configurations whose inner volume is not crossed by any cable or strut in order to place and protect a useful payload (e.g. actuator, micro- controller, energy storage, sensor, depending on the cell type)
- The tensegrity structures that use the most symmetric networks are those with an almost spherical shape
- selected the tensegrity structure that has the smaller number of struts and cables: the icosahedron tensegrity
		- Notes: Icosahedron: Polygon with 20 faces
- It is composed of 6 identical struts and 24 cables of equal length. The cables are organized in 8 equilateral triangles interconnected by 12 vertices and distributed in 4 parallel opposite pairs
- When the icosahedron structure is compressed along a direction orthogonal to any of the four triangle pairs (Fig 2c), it displays maximum deformability and can be col- lapsed to a flat configuration


### Design and Manufacturing
---
- For cables, we use Nin- jaFlex, an elastic material compatible with commercially available fused deposition modeling 3D printers that can withstand 65% of elongation at yield.
- or struts, we use pultruded carbon rods (that are commercially available in different diameters and length)
- The icosahedron tensegrity prototype in Fig. 2c is made of an elastic network of thickness and width of 1 mm and with cables long 4.75 cm each, has a height of 7.8 cm and can be approximated to a sphere of the same diameter, therefore occupying a volume of about 248 cm3
- All cables have the same length and, if shortened, they become more stretched during the assembly (when the struts length is kept constant) and result into a stiffer module.


### Connectivity
---
- Connection points may also serve as a medium to transmit information and energy throughout the robot
- However, at this stage we use only a simple mechanical latching that allows us to assemble cells into a proof-of-concept functional robot
- In this paper, we propose to use a tendon-driven contractive system operated by a servo-motor. Although the servo-motor is a rigid component that can reduce the overall softness of the system [23] and the volume reduction in fully collapsed state, the chosen motor has a small volume (5 cm3) compared to that of the module (248 cm3)
- The contractive mechanism comprises six tendons that connect each vertex of the selected triangular faces to a pulley that is activated by a servo-motor (see Fig 6b). The pulley is placed at the geometrical center of the icosahedron structure (see Fig 6b). When the servo is activated, the pulley starts to rotate wrapping the tendons, which in turn produce a contraction of the icosahedron


### A Crawling Modular Robot
---
- to develop a simple crawling modular robot using peristaltic loco- motion as a proof-of-concept
- The robot is composed of 3 actuated modules connected along the actuated axes with mechanical latching. The three modules are controlled with an external Arduino Uno board using three different signals
-  A driving signal controls the contraction and expansion of a module along the actuated axis. At each step cycle, the three modules contract in sequence from left to right
- This actuation pattern with different speed in con- traction and expansion generates a directional friction on the ground which allows the assembly to move forward.


### Conclusions and Future Work
---
- the proposed design displays many desirable features that could lead to the assembly of a variety of more complex robots with a diverse set of behaviors, other tensegrity structure modules could be considered for specialized func- tions within a heterogeneous modular robot
- the system could benefit from a better integrated actuation system to replace the conventional servo-motor used here as proof of concept: a possible solution could be a contraction system made of shape memory alloys that fit the reticular structure of the modules
- For internal communication, the tensegrity approach could exploit a phenomenon known as mechanotransduction in biology, which is used by cells to activate biochem- ical processes or gene expression. This form of communication could enhance or re- place digital electrical communication by propagating mechanical disturbances that al- ter the function and behavior of the cells.
- Tensegrity simulation tools, such as the NASA Tensegrity Robotics toolkit [25], could be adapted to design and even evolve [20] modular tensegrity robots.

