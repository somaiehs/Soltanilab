## 📚 Project Team
- **Dr. Somaieh Soltani** – Supervisor and Principal Investigator
- **Hadi Khalilpour** – MSc researcher, Principal investigator
  **Dr. Gerhard Wolber** – Scientific Advisor  

# 🧬 NB-Chembl-Multiligand-Predictor

**Evidence-Based Target Discovery Using Naïve Bayes and ChEMBL Data**

This project introduces a Python-based framework for predicting biological targets of drug-like compounds using a **Naïve Bayes classifier trained on ChEMBL bioactivity data**. Unlike traditional models, this tool enables **simultaneous target prediction for multiple ligands**, allowing for evidence-based discovery of **shared targets**, **polypharmacological profiles**, and **repurposing opportunities**.

Developed as part of a Master's thesis of Hadi Khalilpour on repurposing **DMARDs for Alzheimer’s disease**, this pipeline supports **batch ligand input**, **target ranking**, and downstream integration with **molecular docking** and **experimental data from published papers and clinical trials**.


## 🚀 Features

- 🧠 **Naïve Bayes Model** trained on ChEMBL bioactivity data
- 🔍 **Multi-ligand input**: supports prediction for compound sets, not just single molecule
- 📊 **Evidence-based filtering**: targets ranked by both predicted probability (Proba) and supporting literature
- 🧪 **Drug repurposing focus**: optimized for exploring DMARDs in neurodegenerative contexts
- 🧬 **Docking-ready output**: suitable for molecular docking and in-silico validation workflows


## 📚 Project Background

This tool was designed to address a limitation in current similarity-based models: **the inability to analyze multiple ligands simultaneously** based on the original model from Chembl. By aggregating predictions across compounds, this approach allows for:

- Cross-validation of target hypotheses
- Identification of high-confidence shared targets
- Enhanced scalability in drug repurposing workflows

The tool was validated in a case study repurposing **25 DMARDs** for Alzheimer’s disease, using fingerprint-based similarity search, Naïve Bayes classification, and molecular docking.

**Project Novelty**

**Experimental Evidence	Score** is boosted for targets supported by known literature or ChEMBL data
**Multi-Ligand Support**	Targets predicted for multiple ligands receive higher confidence ranking
**This scoring system allows the tool to prioritize**:

     Biologically relevant targets with empirical support

     Shared targets across compound libraries (e.g., DMARDs)

    Docking-ready candidates for further in-silico or in-vitro validation

📌 The scoring logic is fully customizable in the source code and can be adapted to different disease contexts or compound types.
---

## 👥 Contributors

- **Prof. Dr. Somaieh Soltani** – Principal Investigator  
- **Hadi Khalilpour** – MSc Researcher & Developer  
- **Dr. Gerhard Wolber** – Scientific Advisor  

---

## 📦 Requirements

- Python = 3.7.5  
- `rdkit`, `scikit-learn 0.22`, `pandas`, `numpy`, `matplotlib`

