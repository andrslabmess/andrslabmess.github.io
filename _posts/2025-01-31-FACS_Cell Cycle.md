---
title: Cell Cycle
date: 2025-01-31 
categories: [Protocols, FACS]
tags: [FACS]
comments: true 
description: DNA content determination protocol from In Living Color. Protocols in Flow Cytometry and Cell Sorting. R.A. Diamond and S. DeMaggio (Eds.) Springer Lab Manual, 2000, p. 361.
---


#### Reagent and solution
* Propidium Iodide for DNA Content
* *Note:* After running samples with Propidium Iodide the cytometer needs thorough cleaning with 10% bleach and distilled water!
* 70% ethanol
* ribonuclease (100 µg/ml DNase free, Sigma)
* propidium iodide (50 µg/ml in PBS)


## Protocol
* harvest cells. Spin (1200 rpm; 5 min)
* discard supernatant; add 1 ml ' fridge cold' 70% ethanol to 1x10<sup>6</sup> cells while vortexing the cell pellet gently
* fixation (at least 30 min.; 4° C)
* spin (2000 rpm; 5 min) 
* *Note:* once in 70% ethanol, samples may be kept for up to 2 weeks
* discard supernatant and resuspend cells in 1 ml PBS. 
* spin (2000 rpm; 5 min)
* repeat step 5 twice more
* add 100 µl ribonuclease (100 µg/ml, DNase free, Sigma) 
* incubate at room temperature for 5 min
* add 400 µl propidium iodide (50 µg/ml in PBS) 
* *Note:* PI is potentially mutagenic so wear gloves. Before running the samples stained for 
* DNA content the cytometer's linearity, resolution and doublet discrimination capability should be verified. DNA QC kit is necessary and should be ordered from Becton Dickinson (Cat. No. 349523). The kit is composed of :
    *  CEN- chicken erythrocyte nuclei, used in setting cytometer's photomultiplier tube;
    * (PMT) voltages and amplifier gains, and providing information regarding instrument linearity and resolution;
    * CTN - calf thymocyte nuclei, a cycling cell component that allows assessment of proper function of doublet discrimination module (DDM) or pulse processing. Please follow the instructions included in the kit for quality control and set-up of the machine.
  <br>  
* acquire data on a FACScan or FACSCalibur, the cytometer should be triggered on the PI signal. Primary gate is on forward scatter (FSC) against right angle light scatter (SSC).
* a secondary gate should be placed around the single cell population on a pulse area versus pulse width dot plot.
* the measurement of cell cycle parameters can be analyzed by modeling programs which fit the best Gaussian distribution curve to each peak, Go-G1, G2-M and then calculate the resulting S-phase. Modfit software from Verity Software House (Verity@vsh.com) or FlowJo can be used.

