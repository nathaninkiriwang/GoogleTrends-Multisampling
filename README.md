# 📊 Google Trends Verification Study  
**Assessing the Reliability of Google Trends Data in Health and Crime Research**  

## 📌 Overview  
Google Trends (GT) is widely used in **health, social sciences, and economic research**, but its reliability remains questionable due to **limited sampling, normalization, and algorithmic biases**.  

This study replicates two key research papers using **130 samples** per search term to assess the impact of multi-sampling:  
1️⃣ **The Parable of Google Flu** (Lazer et al.) - GT data vs. Flu outbreaks  
2️⃣ **Methamphetamine Study** (Gamma et al.) - GT data vs. Meth-related crime  

By re-evaluating these studies with **multiple GT samples**, we analyze how results fluctuate depending on Google's data extraction methods. We performed the study in R and used QMD notebooks to perform analysis.

---

## 🔬 Key Findings  
✅ Multi-sampling revealed **significant variability** in search trends, leading to inconsistencies in past research.  
✅ **Highly specific search terms (e.g., "early signs of flu") showed greater variability**, making single-sample GT studies unreliable.  
✅ **Methamphetamine search trends** were underestimated in the original study, showing **bias in crime prediction models**.  
✅ Google’s **10-15% sampling method lacks transparency**, leading to **non-reproducible** results.  

📢 **Conclusion:** Single-sample GT studies may be **fundamentally flawed**—multi-sampling should be a requirement for all future GT research.

---

## 🛠 Methods & Techniques  
- **Data Collection:** Automated extraction of **130 Google Trends samples per term** over 130 days.  
- **Dataset Merging:** Cleaning and combining flu/meth-related data for consistency.  
- **Statistical Analysis:** Multi-sample mean comparison, confidence intervals, cross-validation.  
- **Replication of Results:** Reproducing figures from original studies and comparing them with multi-sample averages.  
- **Visualization:** Overlapping trend plots, cross-correlation heatmaps, and comparative error bars.  

---

## 📂 Project Structure  

Google-Trends-Verification/
│── data/                   # Raw and processed Google Trends datasets
│── figures/                # Replicated and multi-sample comparison graphs
│── flu_analysis/           # Quarto project for Google Flu analysis (main QMD)
│── meth_analysis/          # Quarto project for Meth study analysis (main QMD)
│── dataset_merging/        # Quarto project to merge flu & meth datasets
│── README.md               # Project overview & guide
│── LICENSE                 # Open-source license