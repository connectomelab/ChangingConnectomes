---
layout: default
title: "Changing Connectomes: Chapter 7"
date: 2020-08-01
---



### Modelling neuron morphology
Experimental data about neuron morphology in many species is available through the [NeuroMorpho](www.neuromorpho.org) database [1].

[NetMorph](http://www.netmorph.org/) is a C++ environment to simulate neuronal morphogenesis from the perspective of the individual growth cone within axons or dendrites, covering elongation, branching and turning.In this way, neurons with realistic axonal and dendritic morphologies, including neurite curvature, can be generated. Synapses are formed as neurons grow out and axonal and dendritic branches come in close proximity of each other [2]. Compared to CX3D, NetMorph is computationally less expensive, making it useful for theoretical studies and simulating larger networks; on the other hand, NetMorprh is less flexible than CX3D [3].



### Modelling axon growth
Matlab script for [spatial network growth](sng.m). For details on the algorithm, look at Kaiser and Hilgetag (2004)  ([PDF](https://www.dynamic-connectome.org/pubs/Kaiser2004b.pdf), [4])  

Matlab code for simulating the growth of axons and connection establishment can be found [here](CerCor2009.zip). For axonal growth simulations in two or three dimensions, run devsim2d and devsim3d, respectively [5]. 

All previous routines assume that axons grow in a straight line. To test the scenario that axons randomly change direction, we can look at the effect that this would have on overall axon lengths and axon trajectories. Code for modelling curved axonal pathways can be found [here](axon_growth.m) and is described in [6].


### References
[1] Ascoli, G. A., D. E. Donohue and M. Halavi (2007). NeuroMorpho.Org: A central resource for neuronal morphologies. J Neurosci 27(35): 9247-9251.

[2] Koene, R. A., B. Tijms, P. van Hees, F. Postma, A. de Ridder, G. J. Rammers, J. van Pelt and A. van Ooyen (2009). NETMORPH: a framework for the stochastic generation of large scale neuronal networks with realistic neuron morphologies. Neuroinformatics 7(3): 195-210.

[3] Acimovic, J., T. Maki-Marttunen, R. Havela, H. Teppola and M. L. Linne (2011). Modeling of Neuronal Growth In Vitro: Comparison of Simulation Tools NETMORPH and CX3D. EURASIP J Bioinform Syst Biol 2011: 616382.

[4] Kaiser, M., and C. C. Hilgetag. 2004. Spatial growth of real-world networks. Phys Rev E Stat Nonlin Soft Matter Phys 69 (3 Pt 2): 036103

[5] Kaiser, M., C. C. Hilgetag, and A. van Ooyen. 2009. A simple rule for axon outgrowth and synaptic competition generates realistic connection lengths and filling fractions. Cereb Cortex 19 (12): 3001-10.

[6] Kaiser, M. 2017. Mechanisms of Connectome Development. Trends Cogn Sci 21 (9): 703-717.


