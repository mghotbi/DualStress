# 🌾 DualStress (Biotic + Abiotic Stressors)

 **Background and Aim**  
Climate change is intensifying rainfall extremes in major maize-growing regions, increasing the likelihood of concurrent **flooding and herbivory**—a dual stress that disrupts redox balance and undermines yield stability<sup>5,12</sup>.  
While maize responses to individual stresses are well studied, the coordination of **redox buffering between plant genotype and rhizosphere microbiome** under combined stress remains poorly understood<sup>38,82</sup>.  
Repeated domestication and breeding have eroded both genetic and microbial diversity<sup>4,17</sup>, weakening ancestral plant-microbe alliances crucial for oxidative resilience.  

Our preliminary work therefore aimed to:  
1. Quantify how combined flooding-herbivory stress (**DualStress**) alters **soil redox chemistry**, **volatile organic compound (VOC) signaling**, and **rhizosphere microbial structure** along the maize domestication gradient.  
2. Identify **microbial and functional gene signatures** (*nosZ*, *acdS*) linked to redox homeostasis and stress tolerance.

---

## ⚗️ Method

A factorial greenhouse experiment evaluated **10 genotypes** spanning the domestication continuum — from *Zea mays ssp. parviglumis* (wild progenitor), *Zea diploperennis* (wild relative), and landraces (Mexican & American) to modern inbreds and an F₁ hybrid.  

**Treatments:**  
-    Control  
- 💧 Flooding  
- 🐛 Herbivory (induced with *Helicoverpa zea* larvae, a jasmonate-inducing pest)  
- ⚡ **DualStress (flooding + herbivory)**  

**Measurements:**  
- Plant performance: biomass, SPAD chlorophyll index  
- Soil chemistry: pH, Eh, nutrients (Fe²⁺, Mn²⁺, NH₄⁺, NO₃⁻)  
- VOCs: analyzed via SPME-GC-MS  
- Rhizosphere microbiome: 16S, ITS2, *nosZ*, *acdS* sequencing  

Data were processed with **[DspikeIn](https://github.com/mghotbi/DspikeIn)**<sup>83</sup>, and community structure assessed via **PERMANOVA** and **co-abundance networks**<sup>84</sup>.  
**Generalized additive models (GAMs)**<sup>85</sup> tested domestication and treatment effects.  
Cross-domain integration was performed using **mixOmics/DIABLO**<sup>79</sup> to link microbial, soil, plant, and VOC datasets.

---

## 🌍 Results and Discussion

### 🧪 Soil Redox and Nutrient Shifts
DualStress markedly **reduced redox potential**, inducing reductive dissolution of Fe(III) and Mn(IV) oxides and accumulation of Fe²⁺, Mn²⁺, and NH₄⁺, while NO₃⁻ declined — indicating enhanced **denitrification** and weakened buffering capacity.

<p align="center">
  <img src="https://github.com/user-attachments/assets/c80c02a7-1589-4e6c-a647-c8bf8b018b07" width="70%" alt="DualStress schematic">
</p>


<p align="center">
  <em>Figure 1. Overview of Soil Redox and Nutrient Shifts.</em>
</p>

### 🌿 Chlorophyll Content Across the Maize Domestication Gradient

<p align="center">
  <img src="https://github.com/user-attachments/assets/ec8640c2-e2a5-41de-8d92-3f531ed6f7de" width="70%" alt="Chlorophyll (SPAD) content across maize domestication gradient">
</p>

<p align="center">
  <em>Figure 1. Chlorophyll (SPAD) index of maize genotypes spanning the domestication gradient under control (light) and DualStress (dark) conditions.  
  Wild and landrace genotypes maintained significantly higher chlorophyll levels compared to inbreds and hybrids (letters denote Tukey’s HSD groups, P &lt; 0.05), indicating stronger physiological resilience to stress.</em>
</p>

---

Wild and landrace maize retained higher chlorophyll content under flooding–herbivory stress, reflecting **more efficient photosynthetic performance and antioxidant capacity**.  
Modern inbreds and hybrids exhibited **reduced chlorophyll retention**, consistent with diminished stress tolerance and weakened redox homeostasis.

---

###  Volatile Signaling and Genotype Responses
Wild and landrace genotypes emitted a broader and richer blend of stress volatiles (e.g., **trans-α-bergamotene**, **(E)-β-farnesene**, **caryophyllene**, **indole**) than modern lines, supporting **semiochemical** signaling and **microbe-mediated communication**<sup>5,86</sup>.  
However, VOC spectra alone could not explain resilience differences, emphasizing the need for **direct ROS/RNS phenotyping**.

<p align="center">
  <img src="https://github.com/user-attachments/assets/599291f9-714c-41c6-bd20-89b6bf8ebdc5" width="70%" alt="VOC emission profiles">
</p>

<p align="center">
  <em>Figure 2. Genotype-specific VOC emission profiles under DualStress. Wild and landrace maize emit a broader and more diverse suite of stress-induced volatiles compared to modern hybrids, reflecting stronger antioxidant and signaling capacity.</em>
</p>



### 🌱 Microbial and Functional Responses
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

## 🕸️ Network Complexity and Functional Connectivity

<p align="center">
  <img src="https://github.com/user-attachments/assets/761638fa-c182-4415-8340-91cdb0d80062" width="75%" alt="Microbial network complexity across domestication gradient">
</p>

<p align="center">
  <em>Figure 5. ancestral genotypes maintain dense microbial interaction networks.  
  Wild and landrace genotypes exhibit highly connected, hub-rich networks, whereas inbreds and hybrids display simplified, fragmented structures with reduced centrality and modularity.  
  The loss of network connectivity reflects erosion of cooperative microbial interactions linked to redox buffering and stress resilience.</em>
</p>


Network analyses revealed that **ancestral genotypes maintain dense microbial interaction networks** with high harmonic centrality and node connectivity, supporting robust redox regulation.  
In contrast, **modern hybrids exhibit fragmented and less connected networks**, suggesting a loss of functional redundancy and cooperative buffering capacity.  
These results indicate that **network complexity is a key ecological signature of oxidative resilience** across maize evolution.

---

### 🔬 Cross-Domain Integration and Redox-Active Taxa


<p align="center">
  <img src="https://github.com/user-attachments/assets/239105e9-2d84-4217-85d2-2dc365d48a25" width="70%" alt="DIABLO cross-domain integration of plant, soil, microbial, and VOC data">
</p>

<p align="center">
  <em>Figure 4. DIABLO integration linking microbial, soil, plant, and VOC datasets.  
  Cross-domain correlations reveal coordinated shifts in redox-active traits under DualStress.  
  An <i>Anaeromyxobacter</i> ASV correlated with Fe²⁺ and Mn²⁺ concentrations, suggesting a role in coupled Fe–N redox cycling and oxidative stress mitigation.</em>
</p>


DIABLO integration highlighted **tight coupling among plant physiology, soil redox chemistry, and microbiome structure**.  
An *Anaeromyxobacter* ASV strongly co-varied with Fe²⁺ and Mn²⁺ levels, indicating participation in **metal- and nitrogen-linked redox buffering**.  
These results underscore that oxidative resilience arises from **genotype × microbiome × environment** interactions coordinating system-level redox homeostasis.

---

### 🌾 Conclusions
Ancestral genotypes retain stronger antioxidant signaling and microbially mediated stress-buffering networks.  
Domestication has simplified the rhizosphere, reducing **microbial network complexity** and **functional diversity** essential for oxidative resilience.  
Future work will directly quantify **ROS/RNS in maize roots** and integrate **metagenomic/metatranscriptomic** data to map active microbial pathways tied to host antioxidant systems.

> **Takeaway:** Oxidative resilience arises from *genotype × microbiome × environment* interactions — a foundation for **holobiont-guided, redox-resilient breeding**.

---

## 📂 Data Availability

 data supporting this study are available :  
👉 [**Dataset**](https://drive.google.com/drive/folders/1jFDAiELmzVlpS2oloEV73UagBMa4jPuP?usp=sharing)
