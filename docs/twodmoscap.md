---
sidebar_position: 3
---

# Two-Dimensional MOS Capacitor

In this article, we will explore the two-dimensional MOS capacitor, 
the counterpart of the more familiar MOS capacitor.

The figure below shows the structure of the device we will analyze.
The structure has a sheet of semiconductor sandwiched between two insulators with gate electrodes.
For the present analysis, we will take up the case of a symmetric double-gate structure, i.e.,
both the insulators are identical (in thickness and dielectric constant), and an identical bias is 
applied to both the gate electrodes. 
Extending the analysis presented here to the asymmetric case should be straightforward and  trivial.

## Some Initial Observations

The semiconducting layer is ultra-thin in nature. 
For analysis using classical electrostatics we will assume the thickness of the semiconductor to be zero.
This assumption is reasonably valid in the monolayer limit but might cease to be valid in a few-layer system.
The zero thickness of the semiconductor ensures that there is no electrostatic potential variation along its thickness !!
This contrasts with the regular MOS capacitor, where electrostatic potential can vary along its body,
giving rise to what is called "band-bending" in a 3D MOS capacitor. 
The 2D MOS capacitor, on the other hand, has no band bending. 
It only has what we would call "band-movement". 
The semiconducting layer, therefore, is at a single potential given by $\phi_s$.
The central problem we will try to solve is to find this potential, $\ph_s$ 
given the gate bias and the properties of various materials in the device.
Later, when we look at transistors, this potential will vary along the lateral direction of the semiconductor.
