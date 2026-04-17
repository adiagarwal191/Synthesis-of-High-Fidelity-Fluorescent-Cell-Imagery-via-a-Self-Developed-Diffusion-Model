# Synthesis of High-Fidelity Fluorescent Cell Images via a Self-Developed Diffusion Model

This repository contains the code and documentation for my final year project at the University of Birmingham, where I developed and trained a custom Denoising Diffusion Probabilistic Model (DDPM) to generate high-quality synthetic images of fluorescently dyed cells.

## Overview

Diffusion models are a class of generative models that iteratively denoise random noise to produce data samples. In this project, I applied a DDPM to the domain of biological imaging, aiming to generate realistic microscopy images of fluorescently stained cells. The model was trained on a curated dataset of cell images, and its performance was evaluated through qualitative visual inspection and structural similarity metrics.

## Features

- Custom implementation of a DDPM architecture in PyTorch
- Preprocessing pipeline for microscopy images, including normalization and resizing
- Training framework with logging and checkpointing
- Support for image sampling, interpolation, and noise level visualisation

## Dataset

The dataset used consisted of grayscale fluorescent microscopy images collected from publicly available biological image repositories. Images were standardized to a fixed size and normalized for training.

You can access the dataset here:  
https://www.ebi.ac.uk/biostudies/bioimages/studies/S-BIAD847

## How to Use

1. Download the dataset and pre-process it to your preference.
2. Save the dataset to an appropriate path.
3. Adjust hyperparameters in the notebook to match your dataset settings.
4. Run the notebook sequentially to train and sample from the model.

## Acknowledgements

- Based on concepts from DDPM by Ho et al. (2020)
- Inspired by implementation styles from Hugging Face and PyTorch examples
- Supervised by Dr. Alexander Krull, School of Computer Science, University of Birmingham

## License

Shield: [![CC BY-NC-SA 4.0][cc-by-nc-sa-shield]][cc-by-nc-sa]

This work is licensed under a
[Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png
[cc-by-nc-sa-shield]: https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-lightgrey.svg
