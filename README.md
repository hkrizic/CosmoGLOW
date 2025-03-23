# CosmoGLOW: Normalizing Flow-Based Modeling for Detecting Ionizing Sources within H II Regions

This repository contains the **CosmoGLOW**-code, developed for my master's thesis at ETH Zürich:

**Normalizing Flow-Based Modeling for Detecting Ionizing Sources within H II Regions**

![Presentation1](https://github.com/user-attachments/assets/5454c9b8-177f-45c0-ad4a-eac9aed247bf)


The project applies conditional normalizing flows to model the distribution of ionizing sources (halos) within ionized regions (H II bubbles) in the early universe. The approach utilizes the GLOW architecture and demonstrates improvements over standard Gaussian assumptions.

## Repository Structure

```
├── mock_data/                     # Mock dataset: few extracted bubbles from a pyC2Ray slice (at z~9.304) for training and sampling
├── 24022025.pth                   # Trained model checkpoint (approx. epoch 3000)
├── CosmoGLOW_massinference.ipynb  # Inference: sample candidate masses, compute log-likelihoods, and estimate most likely mass
├── CosmoGLOW_sampling.ipynb       # Sampling from the trained model
├── CosmoGLOW_training.ipynb       # Model training 
├── README.md                      # Project overview and documentation
├── bubble_extraction.ipynb        # Extract bubble patches from xfrac and halo catalogues
```


## Requirements

- Python 3.9.18
- PyTorch 2.1.0
- NumPy 1.26.4
- Matplotlib 3.9.2
- SciPy 1.12.0

These versions have been tested and confirmed to work. Newer versions may also be compatible.

## Acknowledgments

This project was conducted at ETH Zürich, Institute for Particle Physics and Astrophysics. It was supervised by:

- Prof. Dr. Alexandre Réfrégier
- Dr. Michele Bianco

## Contact

For inquiries related to this work, please contact Hrvoje Križić (hkrizic [at] ethz.ch)
