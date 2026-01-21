# DPNet: Diffusion-Driven Dynamic Brain Network Modeling

This repository provides the official implementation of DPNet,
a diffusion-based framework for dynamic brain network analysis using resting-state fMRI data.

## Overview
Modeling dynamic brain networks is challenging due to severe noise in BOLD signals, 
inter-subject variability, and unstable functional connectivity patterns. 
DPNet addresses these issues by integrating diffusion-based denoising with adaptive brain connectivity modeling, 
enabling the learning of robust dynamic brain representations for neurological disorder classification.

## Environment
- Python >= 3.8
- PyTorch >= 1.12
- CUDA >= 11.7 

## Install dependencies:

- pip install -r requirements.txt

## Data Preparation
Experiments are conducted on the ADNI and ABIDE datasets.
- ADNI(http://adni.loni.ucla.edu)
- ABIDE(http://fcon_1000.projects.nitrc.org/indi/abide/)

Each dataset should be preprocessed and stored in .npy format with the following structure:
- timeseries: shape (N, T, ROI)
- corr: shape (N, ROI, ROI)
- label: shape (N,)

## Training
Train DPNet on the ADNI or ABIDE dataset:
- python main_pre.py

## Citation
If DPNet is useful for your research, please cite this paper. A formal manuscript describing DPNet is currently in preparation.
