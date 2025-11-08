# 🌾 DualStress (Biotic + Abiotic Stressors)

 **Background and Aim**  
Climate change is intensifying rainfall extremes in major maize-growing regions, increasing the likelihood of concurrent **flooding and herbivory**—a dual stress that disrupts redox balance and undermines yield stability<sup>5,12</sup>.  
While maize responses to individual stresses are well studied, the coordination of **redox buffering between plant genotype and rhizosphere microbiome** under combined stress remains poorly understood<sup>38,82</sup>.  
Repeated domestication and breeding have eroded both genetic and microbial diversity<sup>4,17</sup>, weakening ancestral plant–microbe alliances crucial for oxidative resilience.  

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
- VOCs: analyzed via SPME–GC–MS  
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
  <em>Figure 1. Overview of DualStress experimental design integrating plant, soil, and microbial responses.</em>
</p>

![Redox shifts](<img width="432" height="199" alt="Image" src="https://github.com/user-attachments/assets/c80c02a7-1589-4e6c-a647-c8bf8b018b07" />)

---

### 🌸 Volatile Signaling and Genotype Responses
Wild and landrace genotypes emitted a broader and richer blend of stress volatiles (e.g., **trans-α-bergamotene**, **(E)-β-farnesene**, **caryophyllene**, **indole**) than modern lines, supporting **semiochemical** signaling and **microbe-mediated communication**<sup>5,86</sup>.  
However, VOC spectra alone could not explain resilience differences, emphasizing the need for **direct ROS/RNS phenotyping**.

![VOC profiles](figs/Fig1B_VOC.png)

---

### 🌱 Microbial and Functional Responses
Wild and landrace maize maintained higher chlorophyll content and distinct microbial profiles.  
PERMANOVA confirmed significant **genotype × treatment** effects on both bacterial/archaeal and fungal communities.  
Fungal richness and *nosZ*/*acdS* gene abundance **declined along domestication**, revealing erosion of redox-buffering microbial functions.

![Fungal richness]([Mitra_Figure2_DFG_reduced4.pdf](https://github.com/user-attachments/files/23432305/Mitra_Figure2_DFG_reduced4.pdf))

Network analyses showed that **wild maize harbored hub-rich, highly connected microbiomes**, whereas hybrids exhibited **simplified and redundant networks**.

![Network complexity](figs/Fig3_networks.png)

---

### 🔬 Cross-Domain Integration and Redox-Active Taxa
DIABLO integration revealed tight linkages between microbial, soil, plant, and VOC traits.  
An *Anaeromyxobacter* ASV correlated with Fe²⁺ and Mn²⁺, suggesting a role in **metal- and nitrogen-coupled redox cycling**—oxidizing root-derived C while reducing Fe and nitrate, thus stabilizing redox potential and mitigating oxidative stress<sup>87</sup>.

![DIABLO integration](figs/Fig4_DIABLO.png)

---

### 🌾 Conclusions
Ancestral genotypes retain stronger antioxidant signaling and microbially mediated stress-buffering networks.  
Domestication has simplified the rhizosphere, reducing **microbial network complexity** and **functional diversity** essential for oxidative resilience.  
Future work will directly quantify **ROS/RNS in maize roots** and integrate **metagenomic/metatranscriptomic** data to map active microbial pathways tied to host antioxidant systems.

> **Takeaway:** Oxidative resilience arises from *genotype × microbiome × environment* interactions — a foundation for **holobiont-guided, redox-resilient breeding**.

---

## 📂 Data Availability

All data supporting this study are available via Google Drive:  
👉 [**Download Dataset**](https://drive.google.com/drive/folders/1jFDAiELmzVlpS2oloEV73UagBMa4jPuP?usp=sharing)

or through the main GitHub repository:  
🔗 [https://github.com/mghotbi/DspikeIn](https://github.com/mghotbi/DspikeIn)
