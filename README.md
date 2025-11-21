
 
![image](https://github.com/JIENWU/CaPPI-code/blob/main/CaPPI%20workflow.png)
 
# CaPPI: A Cross-Attention-Based Deep Learning Framework for Predicting Cancer-Related Protein–Protein Interactions

![Workflow](https://github.com/JIENWU/CaPPI-code/blob/main/CaPPI%20workflow.png)

---

## Overview
**CaPPI** (Cancer-associated Protein–Protein Interaction predictor) is a deep learning framework designed to predict cancer-related protein–protein interactions (PPIs).  
The model integrates **Diversified Random Walk (DRW)** for network topology learning, **Gated Convolutional Neural Networks (GCNN)** for sequence feature extraction, and a **Cross-Attention Mechanism (CAM)** for multi-view feature fusion.  
By jointly leveraging sequence semantics, structural topology, and inter-feature dependencies, CaPPI provides an interpretable and biologically meaningful approach for uncovering novel cancer-associated PPIs.

---

## Framework Architecture
The CaPPI workflow consists of the following major components:

1. **Data Acquisition and Preprocessing**  
   Construction of a high-confidence cancer-specific PPI network by integrating curated and experimentally validated interactions.

2. **Diversified Random Walk (DRW)**  
   Captures heterogeneous topological features from the PPI network through multi-path random walks with diverse transition probabilities.

3. **Gated Convolutional Neural Network (GCNN)**  
   Extracts biologically meaningful local sequence patterns while adaptively filtering noise via gated convolution operations.

4. **Cross-Attention Mechanism (CAM)**  
   Dynamically aligns and fuses topological and sequence representations to enhance multi-modal feature learning.

5. **Prediction Module (MLP)**  
   Uses a fully connected neural network to estimate the interaction probability between protein pairs.

---

## Repository Structure

├── CAM/ # Cross-Attention Mechanism implementation
├── Cross attention/ # Fusion module source code
├── DRW/ # Diversified Random Walk algorithm
├── GCNN/ # Gated Convolutional Neural Network
├── MLP/ # Multi-Layer Perceptron prediction module
├── CaPPI workflow.png # Framework architecture diagram
├── README.md # Project documentation
└── .gitattributes # Git configuration


---

## Key Features
- Integrates **graph topology**, **sequence semantics**, and **attention fusion** in a unified model.  
- Employs **diversified random walks** to enhance structural representation of protein nodes.  
- Provides **biologically interpretable predictions**, validated through **case studies** and **molecular docking** experiments.  
- Outperforms conventional machine-learning baselines in stability and robustness.  
- Includes **ablation analysis** demonstrating the critical roles of DRW, GCNN, and CAM modules.

---

## Citation
If you use **CaPPI** in your research, please cite:

> **Yilu Si**, et al. *CaPPI: A Cross-Attention-Based Deep Learning Framework for Predicting Cancer-Related Protein–Protein Interactions*. (2025)



