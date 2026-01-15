# Histo-Fusion-Overview
# 🧬 Histo-Fusion: Spatial Omics Integration Pipeline

![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0-orange)
![Scanpy](https://img.shields.io/badge/Scanpy-1.9-green)

## 📌 Overview
**Histo-Fusion** is a comprehensive computational biology pipeline that integrates high-resolution histology images with spatial transcriptomics data. It uses a graph neural network (GNN) approach to infer cellular neighborhoods and ligand-receptor interactions.

## ⚙️ The Pipeline
This repository contains a modular workflow consisting of 19 specialized analysis steps:

| Module | Description |
| :--- | :--- |
| **01-02** | Environment verification and data loading integrity checks. |
| **03-06** | **Preprocessing:** HuBMAP data ingestion, spatial alignment, and simulation. |
| **07-10** | **Model Setup:** Architecture definition and GNN graph construction. |
| **11-12** | **Training:** Deep learning model training and embedding generation. |
| **13-16** | **Analysis:** Visualization, clustering, and biological annotation. |
| **17-19** | **Advanced:** Cellular neighborhoods and Ligand-Receptor analysis. |

## 🚀 Usage
The entire pipeline can be orchestrated via the central CLI tool:

```bash
# Run the full pipeline
python histofusion_cli.py --mode full

# Run specific analysis modules
python s13_visualize_results.py
