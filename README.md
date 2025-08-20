# FT-Transformer with Spiking Neural Head

This repository provides experimental implementations of the **Feature Tokenizer Transformer (FT-Transformer)**, extended with a **Spiking Neural Network (SNN) head** for binary classification tasks. The primary application explored here is **fraud detection** on structured tabular data.

---

## **Motivation**
Transformers have shown strong performance on tabular datasets, yet they often entail high computational and energy costs. By integrating **spiking dynamics** into the prediction head, this work explores whether biologically-inspired computation can enhance efficiency and robustness in fraud detection while maintaining competitive predictive performance.

---

## **Dataset**
Experiments are conducted on the **Bank Account Fraud (BAF) dataset**, introduced in the NeurIPS 2022 competition *Turning the Tables: Biased, Imbalanced, Dynamic Tabular Datasets*.  
- Official source: [Kaggle – Bank Account Fraud Dataset (BAF)](https://www.kaggle.com/datasets/sgpjesus/bank-account-fraud-dataset-neurips-2022)  

---

## **Methodology**
- **Baseline**: FT-Transformer with a standard linear head.  
- **Hybrid Model**: FT-Transformer encoder with an **SNN head**   
- **Optimization Objective**: Hyperparameter tuning with **Optuna**, maximizing *recall under a fixed False Positive Rate (FPR ≤ 5%)*.  

---

## **References**
- Gorishniy, Y., Rubachev, I., Khrulkov, V., & Babenko, A. (2021). *Revisiting Deep Learning Models for Tabular Data*. Advances in Neural Information Processing Systems (NeurIPS). [Paper](https://proceedings.neurips.cc/paper/2021/hash/9d86d4541c1e02e4a30f430f94f4808d-Abstract.html)  
- Jesus, S. G. P., Monteiro, P., & Bizarro, P. (2022). *Bank Account Fraud Dataset: Turning the Tables – Biased, Imbalanced, Dynamic Tabular Datasets*. NeurIPS 2022 Competition Track. [Kaggle](https://www.kaggle.com/datasets/sgpjesus/bank-account-fraud-dataset-neurips-2022)  
- Fang, W., Chen, Y., Ding, J., Chen, D., Yu, Z., Zhou, H., ... & Tian, Y. (2021). *SpikingJelly: An Open-Source Machine Learning Framework for Spiking Neural Network Research*.  

---

## **License**
Released under the terms specified in the [LICENSE](LICENSE).  