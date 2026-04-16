---
title: "✂️ & 🏷️ R-loop"
date: 2026-02-21 
categories: ["Z_Miscellaneous SaS", "Notes"]
tags: ["Sequencing"]
comments: truee
author:  Sarka
description:
---

## Intro

<a href="https://www.activemotif.com/applications-cut-and-tag">CUT&Tag Resource Center</a><br>
<a href="https://www.activemotif.com/catalog/1365/r-loop-service">CUT&Tag-IT® R-loop Service</a><br>
<a href="https://www.activemotif.com/catalog/1376/cut-tag-r-loop-kit">CUT&Tag-IT® R-loop Assay Kit</a><br>
<a href="https://www.activemotif.com/catalog/1383/cut-tag-spike-in-r-loop">CUT&Tag-IT® Spike-In Control, R-loop</a><br>


## 1. Cut & Tag protocol
***Note*** 
<br>
we used reduced volumes of reagents/solvents when we weren't sure if we had enough (specified in Marketa’s protocol)
<br>
<object data= "{{ site.url }}/../uploads/Sarka/protocols/CutAndTag.pdf" width="800" height="800" type='application/pdf'></object>
<br>
<br>
<a href="https://www.activemotif.com/documents/2265.pdf">PDF: Protocol; CUT&Tag-IT™ R-loop Assay Kit</a><br>
<a href="https://www.activemotif.com/documents/2280.pdf">PDF: CUT&Tag-IT®
 Spike-In Control, R-loop</a><br>
<a href="https://www.activemotif.com/documents/2305.pdf">PDF: Counting Cells and Nuclei
for Epigenetic Applications</a><br>


#### Library Preparation for Illumina
* I find this one very usefull 
* it includes also videos with "real life tips" on right side - description of each bellow<br>

<a href="https://www.neb.com/en/products/next-generation-sequencing-library-preparation/library-preparation-for-illumina">Library Preparation for Illumina: text & videos</a><br>

## 2. Concentration

<br>
>
***Qubit & Tapestation***
<br>
For a professional NGS library prep, the standard protocol: <br>
Use the TapeStation for the "Size" and the Qubit for the "Concentration." 
* When pooling libraries for an Illumina run, even a small error in concentration can lead to "index hopping" or uneven data distribution (where one sample gets 90% of the reads and others get 10%).
* Using the TapeStation to check size and the Qubit to check molarity ensures your final calculations for pooling (converting ng/µL to nM) are as accurate as possible. <br>
<br>
***When can you skip one?***
<br>
If you are in a situation where you must choose just one to save time or sample:
* TapeStation only : samples are all the exact same type (e.g., all the same PCR amplicon length) and you have a very high concentration.
* Qubit only: already know exactly what size your fragments are (e.g., a specific 300bp PCR product) and don't need to check for degradation.<br>
*(source: Gemini)*
{: .prompt-tip }
<br>

### 2A. Qubit
***Note***
* protocols are usualy everywhere with Qubit
* there are special tubes for it
<br>
<br>
***Qubit dsDNA Quantification Assay Kits***
1. dsDNA
2. dsDNA: High Sensitivity
3. lower and upper point calibration (S1 and S2)
4. dilution of samples 1:200 : 1 μL + 199 μL
5. units: ng/μL
<br>
<br>
***Workflow***
* samples on ice
* thaw at r.t. (but keep on the ice rest of the time)
* “flick the samples” – to homogenize
* spin down (short spin at r.t. centrifuge)
* mix with buffer (pipet first buffer 199μL and then sample 1μL)
* quick vortex
* incubation (r.t.; 3 min; can differ base of kit)
* measure (ng/μL) + write down a concentrations
* optional: download data on USB
<br>
<br>
<a href="https://documents.thermofisher.com/TFS-Assets/LSG/manuals/MAN0017209_Qubit_4_Fluorometer_UG.pdf">Qubit™ 4 Fluorometer: pg 18-28</a><br>

#### Calculation of dsDNA library concentration
* if you would like to calculate concentration from Qubit
* <a href="https://knowledge.illumina.com/library-preparation/dna-library-prep/library-preparation-dna-library-prep-reference_material-list/000001240" target="_blank">dsDNA library concentration</a><br>
<br>
 

### 2B. Tapestation

<object data= "{{ site.url }}/../uploads/Sarka/protocols/TapeStation.pdf" width="800" height="800" type='application/pdf'></object>

<br>
<br>
>
<a href="https://youtube.com/shorts/ishea7isuG8">Our video protocol for Agilent TapeStation Software 5.1</a><br>
{: .prompt-tip }
<br>
<br>

* <a href="https://hpst.cz/sites/default/files/oldfiles/g2991-90130.pdf">Agilent High Sensitivity D1000 ScreenTape Assay Quick Guide for 4200 TapeStation System</a><br>
* <a href="https://www.youtube.com/watch?v=ZGvCGRxFiuE&t=3s">You Toube: 
TapeStation tutorial - very nicely explained; Workflow: sapmple preparation from 01:00; Workflow: TapeStation from 08:27; Workflow: Software from 09:37</a><br>
* <a href="https://www.youtube.com/watch?v=c-I4aioxMBo">You Toube: Agilent TapeStation: DNA and RNA Applications; Workflow from 14:54</a><br>
* <a href="https://www.malariagen.net/wp-content/uploads/2023/10/GbS04_Agilent_TapeStation.pdf">Agilent TapeStation</a><br>

## 3. Pooling

* <a href="https://support.illumina.com/help/pooling-calculator/pooling-calculator.htm">Pooling Calculator Illumina</a><br>

<br>
![image](uploads/Sarka/protocols/IlluminaPoolingCal.png){: .centre width="400"}
<br>

<br>
>
* concentration from libraries (e.g. Region Molarity [nmol/l])
* elution buffer as diluent for pooling - correct concentration of Tris <br>
{: .prompt-info }

<br>
>
***Novaseq X***
* pool samples equimolarly
* the minimum 5nM to guarantee the best results
* 35 μL per lane (minimum volume); can be higher
* pool in a 1.5 mL low-bind tube
{: .prompt-info }

<br>
>
***Under-represented samples*** <br> 
Example
* pool all experimental samples equimolarly (5nM)
* pool the 4 negative controls at a slightly lower molarity<br>
{: .prompt-info }

<br>
>
It is better to discuss dilution with the genomics center before pooling.<br>
{: .prompt-tip }


<br>
>
Let them know, which assay was used at TapeStation - for their quality assesment (**HS D1000**, or they can try D5000 for longer fragments).
{: .prompt-tip }

<br>

<br>

## Further resources

#### NEBNext® Ultra™ II DNA Library Prep Kit for Illumina®
<a href="https://www.neb.com/en/products/e7645-nebnext-ultra-ii-dna-library-prep-kit-for-illumina?srsltid=AfmBOoqiEkfW6zqIcwvkYSi56rQCwjE8mcNlP18ZxYh8qNVfFuVry5WV">INSTRUCTION MANUAL</a><br>

#### Multiplex Oligos for Illumina Protocol
<a href="https://www.cellsignal.com/learn-and-support/protocols/multiplex-oligos-illumina-dual-index">Click</a><br>

#### Learn about Illumina's Next-Generation Sequencing Workflow
<a href="https://www.youtube.com/watch?v=oIJaA6h2bFM&ab_channel=Illumina">Illumina's Next-Generation Sequencing Workflow</a><br>

#### Calculation of dsDNA library concentration
* <a href="https://knowledge.illumina.com/library-preparation/dna-library-prep/library-preparation-dna-library-prep-reference_material-list/000001240" target="_blank">Click</a><br>
