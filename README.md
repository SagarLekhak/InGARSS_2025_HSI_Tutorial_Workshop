# Hyperspectral Target Detection Tutorial

This repository provides a complete, beginner-friendly yet technically rigorous tutorial on classical statistical hyperspectral target detection. It walks through essential concepts, preprocessing steps, implementation details, and evaluation methods using a real hyperspectral dataset in ENVI format.

The tutorial is organized as a Google Colab notebook and is designed to help students, researchers, and practitioners understand and implement widely used hyperspectral detection algorithms.

---

## 📌 What You Will Learn

By working through this tutorial, you will learn how to:

### **1. Load and Analyze Hyperspectral Data**
- Read ENVI `.hdr` and binary files in Python  
- Visualize and inspect hyperspectral cubes  
- Work with pixel spectra and metadata  

### **2. Implement Classical Target Detection Algorithms**

Full implementations of four well-known statistical detectors:

- **SAM — Spectral Angle Mapper**  
- **MF — Matched Filter**  
- **ACE — Adaptive Cosine Estimator**  
- **CEM — Constrained Energy Minimization**

Each algorithm is implemented from scratch, including:
- Mean-centering steps  
- Covariance estimation  
- Score normalization  
- Pixel-level detection map generation  

### **3. Evaluate Detection Performance**
- Apply custom detection thresholds  
- Generate ROC curves  
- Compare algorithm performance on real target signatures  

### **4. Perform Dimensionality Reduction Using PCA**
- Compute PCA using SVD  
- Examine explained variance and the optimal number of components  
- Project hyperspectral data into reduced-dimensional space  
- Apply detection algorithms in PCA space  
- Reconstruct the HSI from PCA bands and compare performance with the original data  

---

## 📁 Dataset Description
### 🛰️ About the Dataset (RIT SHARE 2012)

The hyperspectral image is from the **RIT SHARE 2012 dataset**, a VNIR hyperspectral collection over controlled target fields with known materials and ground truth. The scene contains several red felt targets and is widely used for benchmarking classical detectors such as **SAM, MF, ACE, and CEM**. The dataset was provided by **Prof. Dr. Emmett J. Ientilucci**.

**Reference:**  
Avery, S., & Schott, J. (2013). *Summary of the 2012 SHARE Data Collection Campaign.* Rochester Institute of Technology, Center for Imaging Science.

Three supporting data files are included (or referenced):

### **Hyperspectral Image (ENVI format)**  
001_0729-1919_rad_GeoRef_THOR_ELM_smoothed 146x84

001_0729-1919_rad_GeoRef_THOR_ELM_smoothed 146x84.hdr

### **Target Signature File**
(Spectral signature of the red target)

Red Felt Refl ASD Reseamp 360 ASCII.txt

### **Ground Truth Class Map**
class_map_envi

class_map_envi.hdr


**Objective:**  
Detect the red felt targets in the hyperspectral scene using classical statistical algorithms in both the spectral and PCA-reduced spaces, and compare their performance using ROC curves.

---

## 📚 Tutorial Structure

### **Step 1 — Preprocessing**
- Load HSI cube  
- Flatten and reshape functions  
- Mean-centering  
- Data exploration  

### **Step 2 — Target Detection Algorithms**
- Implement SAM, MF, ACE, CEM  
- Visualize detection score maps  
- Compute ROC curves using ground truth  
- Compare algorithm performance  

### **Step 3 — PCA-Based Target Detection**
- Compute PCA decomposition  
- Plot explained variance  
- Choose optimal number of components  
- Apply SAM/MF/ACE/CEM in reduced space  
- Reconstruct HSI and verify equivalence with full-dimensional detection  

---

## 🎯 Purpose of This Repository

This repository serves as:
- A teaching tool for hyperspectral imaging and statistical detection  
- A reference implementation for classical target detection methods  
- A hands-on guide for students and researchers working with spectral remote sensing data  
- A practical demonstration of PCA-based dimensionality reduction for HSI  

---
---

## 📢 Presentation

This tutorial will be presented at **InGARSS 2025 — IEEE India Geoscience and Remote Sensing Symposium** in **Bhubaneswar, India**, on **10 December 2025**, by **Prof. Dr. Emmett J. Ientilucci**.

---

## 👤 Authors / Contributors

### **Prepared By:**  
**Sagar Lekhak**  
PhD Student, Chester F. Carlson Center for Imaging Science  
Rochester Institute of Technology, NY, USA  
Email: sl3088@rit.edu  

### **Research Advisor:**  
**Prof. Dr. Emmett J. Ientilucci**  
Gerald W. Harris Professor, Chester F. Carlson Center for Imaging Science  
Rochester Institute of Technology, NY, USA  
Email: ejipci@rit.edu


