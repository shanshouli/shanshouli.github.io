---
name: Deep Learning Pipeline for Neutron Reflectivity Analysis
tools: [PyTorch, NumPy, Pandas, CUDA, HPC, Slurm]
image: https://images.unsplash.com/photo-1553623095-2b4d2819983f?w=800
description: End-to-end ML pipeline automating neutron reflectivity data interpretation with improved CNN model, achieving 12% improvement in SLD profile R² score through optimized HPC training on NVIDIA A100/V100 GPUs.
---

<style>
/* Page-specific font override to use a more standard system stack. */
.markdown-body {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif;
}
</style>


# Deep Learning Pipeline for Neutron Reflectivity Analysis

**Duration:** Jan 2025 – Apr 2025  
**Collaboration:** Oak Ridge National Laboratory  
**Tech Stack:** PyTorch, NumPy, Pandas, CUDA, Slurm, HPC, Linux  
**Paper:** In preparation — link coming soon

## Overview

Developed an end-to-end machine learning pipeline that automates the interpretation of neutron reflectivity (NR) data and infers thin film material structures, in collaboration with Oak Ridge National Laboratory.

## Key Achievements

### 🧠 Model Architecture & Performance
- Leveraged an **improved CNN model** with dropout and spatial dropout for enhanced robustness against noisy experimental inputs
- Achieved **12.0% improvement in SLD profile R² score** compared to prior models
- Obtained **8.7% gain in NR curve R² score** on experimental data
- Significantly improved model fidelity to manual fitting benchmarks

### 📊 Data Engineering
- Employed **Pandas and NumPy** for large-scale NR/SLD dataset cleansing, feature engineering, and statistical normalization
- Implemented vectorized I/O operations that **cut preprocessing time by 65%**
- Handled complex multi-dimensional scientific data with efficient memory management

### ⚡ High-Performance Computing
- Optimized model training on **HPC clusters with NVIDIA A100 & V100 GPUs**
- Utilized **Slurm-managed resource allocation** and CUDA acceleration
- Configured Linux-based virtual environments for reproducibility
- Achieved **55% reduction in runtime** while maintaining consistent results

## Technical Highlights

- **Deep Learning Framework:** PyTorch with custom loss functions for physical constraints
- **GPU Optimization:** Efficient batch processing and memory management for large-scale training
- **Scientific Computing:** Integration with physics-based models and experimental validation

## Impact

This pipeline enables researchers to rapidly analyze neutron reflectivity experiments, reducing interpretation time from hours to minutes while improving accuracy beyond traditional manual fitting methods.
