# 🌾 DualStress 

 **Background and Aim**  
Climate change is intensifying rainfall extremes in major maize-growing regions, increasing the likelihood of **flooding ** stress that disrupts redox balance and undermines yield stability<sup>5,12</sup>.  
While maize responses to individual stresses are well studied, the coordination of **redox buffering between plant genotype and rhizosphere microbiome** under stress remains poorly understood<sup>38,82</sup>.  
Repeated domestication and breeding have eroded both genetic and microbial diversity<sup>4,17</sup>, weakening ancestral plant-microbe alliances crucial for oxidative resilience.  

Our preliminary work therefore aimed to:  
1. Quantify how flooding stress alters **soil redox chemistry**, **volatile organic compound (VOC) signaling**, and **rhizosphere microbial structure** along the maize domestication gradient.  
2. Identify **microbial and functional gene signatures** (*nosZ*, *acdS*) linked to redox homeostasis and stress tolerance.

---

##  Method

A factorial greenhouse experiment evaluated **10 genotypes** spanning the domestication continuum, from *Zea mays ssp. parviglumis* (wild progenitor), *Zea diploperennis* (wild relative), and landraces (Mexican & American) to modern inbreds and an F₁ hybrid.  

**Treatments:**  
-  Control  
- 💧 Flooding  

**Measurements:**  
- Plant performance: biomass, SPAD chlorophyll index  
- Soil chemistry: pH, Eh, nutrients (Fe²⁺, Mn²⁺, NH₄⁺, NO₃⁻)  
- VOCs: analyzed via SPME-GC-MS  
- Rhizosphere microbiome: 16S, ITS2, *nosZ*, *acdS* sequencing  

Data were processed with **[DspikeIn](https://github.com/mghotbi/DspikeIn)**<sup>83</sup>, and community structure assessed via **PERMANOVA** and **co-abundance networks**<sup>84</sup>.  
**Generalized additive models (GAMs)**<sup>85</sup> tested domestication and treatment effects.  
Cross-domain integration was performed using **mixOmics/DIABLO**<sup>79</sup> to link microbial, soil, plant, and VOC datasets.

---

##  Results and Discussion

###  Soil Redox and Nutrient Shifts
Flooding markedly **reduced redox potential**, inducing reductive dissolution of Fe(III) and Mn(IV) oxides and accumulation of Fe²⁺, Mn²⁺, and NH₄⁺, while NO₃⁻ declined, indicating enhanced **denitrification** and weakened buffering capacity.


<p align="center"> <img width="538" height="653" alt="Soil and plant trait dynamics along maize domestication" src="https://github.com/user-attachments/assets/722cc489-2505-4042-bd2f-d93fe3d4f466" /> </p> <p align="center"> <em><b>Figure.1 </b> Soil physicochemical properties and plant chlorophyll content (SPAD) across the maize domestication gradient under control and flooding conditions. Data illustrate shifts in nutrient availability and plant performance from wild progenitors to modern hybrids, reflecting progressive optimization of redox and nutrient dynamics. </em> </p>


Wild and landrace maize retained higher chlorophyll content under flooding stress, reflecting **more efficient photosynthetic performance and antioxidant capacity**.  
Modern inbreds and hybrids exhibited **reduced chlorophyll retention**, consistent with diminished stress tolerance and weakened redox homeostasis.

---

###  Volatile Signaling and Genotype Responses
Wild and landrace genotypes emitted a broader and richer blend of stress volatiles (e.g., **trans-α-bergamotene**, **(E)-β-farnesene**, **caryophyllene**, **indole**) than modern lines, supporting **semiochemical** signaling and **microbe-mediated communication**<sup>5,86</sup>.  
However, VOC spectra alone could not explain resilience differences, emphasizing the need for **direct ROS/RNS phenotyping**.


<p align="center"> <img width="500" height="910" alt="Volatile organic compound profiles across domestication and flooding" src="https://github.com/user-attachments/assets/300c21ad-cda6-4068-91d2-86b44b68c3ba" /> </p> <p align="center"> <em><b>Figure.2 </b> Volatile organic compound (VOC) emission profiles across the maize domestication gradient under control and flooding conditions. The heatmap shows relative emission intensities of individual VOCs (rows) across genotypes (columns). Flooding markedly alters both the abundance and diversity of emitted compounds, with wild and landrace maize maintaining broader and more complex VOC repertoires compared to modern hybrids. </em> </p>
Domestication gradient: Wild progenitor → Wild relative → Mexican landrace → American landrace → Inbred landrace → Inbred modern → Conventional hybrid


###  Microbial and Functional Responses
Wild and landrace maize maintained higher chlorophyll content and distinct microbial profiles.  
PERMANOVA confirmed significant **genotype × treatment** effects on both bacterial/archaeal and fungal communities.  
Fungal richness and *nosZ*/*acdS* gene abundance **declined along domestication**, revealing erosion of redox-buffering microbial functions.


<p align="center">
  <img src="https://github.com/user-attachments/assets/f6ee1e8f-36bd-4eb8-85dd-a3248e9558cc" width="80%" alt="PCoA and functional gene trends (nosZ, acdS)">
</p>

<p align="center">
  <em>Figure 3. (A) PCoA of bacterial (16S) and fungal (ITS) communities showing clear separation by treatment (T) and domestication (D).  
  (B) Relative abundance of *nosZ* (denitrifiers), *acdS* (ACC deaminase producers), 16S rRNA (bacterial), and ITS (fungal) genes modeled using GAMs (±95% CI).  
  (C) Core fungal families (≥80% prevalence, ≥10 reads) across maize domestication groups and stress treatments.</em>
</p>


Wild and landrace genotypes supported distinct bacterial and fungal assemblages under DualStress, with higher *nosZ* (denitrification) and *acdS* (ACC deaminase) abundance compared to inbreds and hybrids.  
This pattern suggests that **ancestral maize lines retain stronger microbial partners for redox regulation and stress mitigation**, whereas modern breeding has led to **simplified, functionally constrained microbiomes**.



Network analyses showed that **wild maize harbored hub-rich, highly connected microbiomes**, whereas hybrids exhibited **simplified and redundant networks**.

##  Network Complexity and Functional Connectivity

<p align="center"> <img width="782" height="457" alt="Microbial network topology across maize domestication" src="https://github.com/user-attachments/assets/39f1c117-bfed-4d51-b53e-4fc34fdb4505" /> </p> <p align="center"> <em><b>Figure 5.</b> Ancestral genotypes maintain dense and functionally integrated microbial networks. Wild and landrace maize exhibit highly connected, hub-rich communities with elevated degree, closeness, and effective size, whereas inbreds and hybrids display simplified, fragmented structures with reduced centrality and modularity. The progressive loss of network connectivity reflects the erosion of cooperative microbial interactions underpinning redox buffering and stress resilience.</em> </p>

Network analyses revealed that **ancestral genotypes maintain dense microbial interaction networks** with high harmonic centrality and node connectivity, supporting robust redox regulation.  
In contrast, **modern hybrids exhibit fragmented and less connected networks**, suggesting a loss of functional redundancy and cooperative buffering capacity.  
These results indicate that **network complexity is a key ecological signature of oxidative resilience** across maize evolution.

---

###  Cross-Domain Integration and Redox-Active Taxa

<p align="center"> <img width="673" height="648" alt="DIABLO cross-domain integration of plant, soil, microbial, and VOC data" src="https://github.com/user-attachments/assets/3fe69122-781f-4c02-92ff-0bf9e096f2d0" /> </p> <p align="center"> <em><b>Figure 4.</b> Multi-omics integration using DIABLO reveals cross-domain linkages among microbial, soil, plant, and VOC datasets under combined stress. Positive (red) and negative (blue) correlations highlight coordinated regulation of redox-active features across trophic levels. Notably, an <i>Anaeromyxobacter</i> ASV co-varied with Fe²⁺ and Mn²⁺ concentrations, indicating its role in Fe-N coupled redox buffering and oxidative stress mitigation.</em> </p>


Cross-domain integration uncovered tight coupling among plant physiology, soil redox chemistry, and microbiome structure.
An Anaeromyxobacter ASV exhibited strong covariance with Fe²⁺ and Mn²⁺ levels, implicating it in metal- and nitrogen-linked redox regulation.
These findings demonstrate that oxidative resilience in maize arises from genotype × microbiome × environment interactions that collectively stabilize rhizosphere redox homeostasis.


---

### 🌾 Conclusions


Ancestral genotypes retain stronger antioxidant signaling and microbially mediated stress-buffering networks.  

Domestication has simplified the rhizosphere, reducing **microbial network complexity** and **functional diversity** essential for oxidative resilience.  



---

## 📂 Data Availability

 data supporting this study are available :  

© 2025 Mitra Ghotbi. All rights reserved.
The data contained herein remain the intellectual property of the author.
Requests for access or collaboration should be directed to the author.

 [**Dataset**](https://drive.google.com/drive/folders/1jFDAiELmzVlpS2oloEV73UagBMa4jPuP?usp=sharing)

