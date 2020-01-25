# Introduction

Phactory yields phages with toxicity levels that allow for oral administration to the patient. However, oral delivery requires protection of the phages from rapid degradation in the acidic gastric juice, while direct intravenous application requires additional purification steps. To overcome these hurdles, we prototyped two 3D-printed fluidic devices that each can be assembled for less than $5.

For oral application, we built the Phagecapsulator, a nozzle to encapsulate the phages in monodisperse calcium-alginate microspheres that protect them in the stomach. For intravenous administration, we can purify the bacteriophages from the remaining cell-extract via fractionation in a pressure-driven size-exclusion Phactory-Purificator filter system.

## Phage-Encapsulator
### Motivation

As in many manufacturing processes, packaging of our produced phages is the final step of Phactory. Packaging provides long-term storability and ensures a clean and safe product for patients. Lacking access to commercial bioencapsulation devices such as the Inotech Encapsulator IER-50, available at $10,000, we engineered Phage-Encapsulator, an affordable device for encapsulating phages in monodisperse alginate spheres (1).

Requiring only standard parts, phage solution, alginate and compressed air, Phage-Encapsulator makes phage packaging accessible to non-specialized laboratories. The throughput is sufficient to produce encapsulated phages for oral application on-site in less than 2 hours.
Overall design

The core part of the Phage-Encapsulator consists of a dispensing tip that is continuously fed with phage containing alginate solution by a syringe pump. The dispensing tip is surrounded by a chamber connected to a compressed air supply to create a steady stream of air around the tip that shears off a jet of monodisperse droplets, smaller than the diameter of the tip. The alginate droplets are sprayed into a Calcium-Chloride bath where the rapid crosslinking reaction occurs.

<p align="center">
<img width="49%" src="http://2018.igem.org/wiki/images/c/c6/T--Munich--hardware_draw1.png" alt="A generic square placeholder image with  ounded corners in a figure.">
<img width="49%" src="http://2018.igem.org/wiki/images/b/be/T--Munich--hardware_draw2.png" alt="A generic square placeholder image with rounded corners in a figure.">
</p>

### Individual Parts:
#### Alginate Solution

The negatively charged polysaccharide alginate is commonly used for cell encapsulation or as food additive. Alginate undergoes strong shrinking when the pH of the environment drops below its pKa (2). Due to its pKa of ~3.5 this is the case in gastric fluid with a pH of 1 – 2. These properties render alginate spheres an ideal delivery substrate, protecting the phages in the stomach and releasing them in the basic milieu of the intestinal tract. As a tradeoff between alginate viscosity and gel strength, we found that a mixture of 1.8% high viscosity alginate (Art.-No. 9180.1, ROTH) and 0.2 low viscosity alginate (A1112, Sigma Aldrich) represents a good compromise.

### Nozzle
Our final design of the nozzle is shown in Interactive Figure 1. It consists of a chamber that can be connected to a pressure supply via a universial tube adapter. Consisting of two parts, the nozzle does not get in contact with the phage solution, so it can be reused. The dispensing tip can be easily inserted via a Luer-lock adapter and lines up precisely with the nozzle orifice. A centering aid is located behind the orifice to reduce variances in cannula alignment, while the air stream is not disturbed unequally by its symmetric shape. At a given air pressure, the orifice diameter determines the velocity of the air stream and consequently the droplet diameter.

### Calcium bath
Rapid gelation of the phage-containing alginate droplets was obtained in a 10 mM MgSO4 solution with 1.8% CaCl2. Aggregation of alginate droplets was prevented by continuous stirring during droplet generation with a magnet stirrer.

### Syringe pump
In our experiments we used a commercial syringe pump from TSE Systems (type 540060) to create a continuous alginate stream. We designed our nozzle to be compatible with other types of syringe pumps, including open-source solutions.

### Pressure supply
As a pressure supply we used the house gas line, reduced to 1 bar. If not available, the universial tube adapter ensures compatibility to alternative pressure supplies, including portable, open-source solutions.
Part List

- syringe (1ml Braun Omnifix)
- dispensing Tip (ID 0.51mm, Vieweg)
- syringe pump
- pressure supply
- pneumatic tubing
- 4x M3x20 screws + nuts
- 3D printed nozzle (PMMA)

### Results

Our results show that after 1 hour incubation in simulated gastric fluid, active phages are successfully released in simulated intestinal fluid. Within the limited time frame of the iGEM competition we were able to show storability of these alginate spheres with constant phage activity at 4°C for four weeks, while stability for several months was shown in the literature (3).

<p align="center">
<img width="49%" src="http://2018.igem.org/wiki/images/8/84/T--Munich--Results_brightfield_droplet2_hardware.png" />
<img width="49%" src="http://2018.igem.org/wiki/images/9/9c/T--Munich--Results_Droplets_zstack-400_8bit.gif"
</p> 
  

In order to achieve defined phage concentrations and therefore defined doses, we optimized the monodispersity of our alginate droplets.

In our initial attempts to create alginate droplets the size within a batch often varied significantly. Additionally, due to aggregation a lot of droplets were lost. Optimization of parameters such as flow rate, alginate concentration and N2 pressure led to an increase of monodispersity for all tested sizes (50-300 μm). Specifically, an alginate concentration of 1.8 % alginate and 0.2 % low-viscosity alginate proved to be ideal. Pressure and flow rate determine the droplet sizes.
![](http://2018.igem.org/wiki/images/3/38/T--Munich--Results_droplet_optimization.png)

### Bacteriophages Encapsulated In Alginate Can Withstand Gastric Acid 


The main problem of oral application is the acidic environment in the gastric fluid, necessitating protective measures against degradation. The other requirement of phage protection is the release of functional phages in the intestines. For this reason we compared the behavior of the encapsulated phages and non-encapsulated phages in simulated gastric fluid (SGF) and simulated intenstinal fluid (SIF).

In SGF, the number of active non-encapsulated phages decreases by more than 99.99 % within an hour. This shows the urgent need of a form of protection against degradation to make oral application of bacteriophages possible. As a reference, we used phages that were chemically released by citrate from alginate droplets.

![](http://2018.igem.org/wiki/images/4/4f/T--Munich--Results_Joe_SGF_Phages.png)



In comparison, the encapsulated phages were tested in SGF for the same time as the non-encapsulated phages. Afterwards, the same droplets were exposed for two hours to simulated intestinal fluid to test the release of functional bacteriophages in this environment.

The encapsulated phages were barely released in an hour of exposure to SGF. After transfering the capsules to SIF the number of active phages reached that of the undegraded reference. This indicates that the encapsulation of bacteriophages in alginate capsules enables the possibility of an oral application. Further experiments could test the alginate capsules in an animal model system.
 ![](http://2018.igem.org/wiki/images/a/a2/T--Munich--Results_Droplets_phages.png)



## References
<ol>
<li> <a href=https://doi.org/10.1016/j.biomaterials.2009.07.034>Chan, A. W., &amp; Neufeld, R. J. (2009). Modeling the controllable pH-responsive swelling and pore size of networked alginate based biomaterials. Biomaterials, 30(30), 6119–6129. </a></li>
<li> <a href=https://doi.org/10.1016/j.ab.2007.10.045>Kwon, Y.-C., Hahn, G.-H., Huh, K. M., &amp; Kim, D.-M. (2008). Synthesis of functional proteins using Escherichia coli extract entrapped in calcium alginate microbeads. Analytical Biochemistry, 373(2), 192–196. </a></li>
<li> <a href=https://doi.org/10.1038/srep41441>Colom, J., Cano-Sarabia, M., Otero, J., Aríñez-Soriano, J., Cortés, P., Maspoch, D., &amp; Llagostera, M. (2017). Microencapsulation with alginate/CaCO3: A strategy for improved phage therapy. Scientific Reports, 7(1). </a></li>
</ol>
