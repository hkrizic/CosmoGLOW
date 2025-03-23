# CosmoGLOW: Normalizing Flow-Based Modeling for Detecting Ionizing Sources within H II Regions

This repository contains the CosmoGLOW-code, written for my master's thesis project at ETH Zürich:

**Normalizing Flow-Based Modeling for Detecting Ionizing Sources within H II Regions**

![Screenshot 2025-03-23 at 19 10 56](https://github.com/user-attachments/assets/1d3df5f9-0e1d-4e50-850f-176f80b3d7e4)

The project applies conditional normalizing flows to model the distribution of ionizing sources (halos) within ionized regions (H II bubbles) in the early universe. The approach utilizes the GLOW architecture and demonstrates improvements over standard Gaussian assumptions.

## Repository Structure

```
├── mock_data/                    # Some mock data to train the model and try the sampling (extracted bubbles from pyC2Ray)
├── CosmoGLOW_sampling.ipynb      # Training script (feel free to adjust hyperparameters)
├── CosmoGLOW_training.ipynb      # Sampling from the trained model
├── CosmoGLOW_massinference.ipynb # Sampling n Masses, obtaining maximum log-likelihood -> Mass-Inference
├── README.md                     # Project description
├── 24022025.pth                  # Model checkpoint at epoch~3000
```

## Key Features

- Training of conditional normalizing flows based on the GLOW architecture
- Sampling conditioned on bubble geometry using ray-based descriptors and log-mass
- Enforced sampling within bubble contours to ensure physical consistency
- Density visualization via 2D histograms (64x64 grid)

## Requirements

- Python 3.9+
- PyTorch
- NumPy
- Matplotlib
- SciPy

## Usage
### TODO


## Acknowledgments

This project was conducted at ETH Zürich, Institute for Particle Physics and Astrophysics. It was supervised by:

- Prof. Dr. Alexandre Réfrégier
- Dr. Michele Bianco

## Contact

For inquiries related to this work, please contact Hrvoje Križić (hkrizic [at] ethz.ch)
