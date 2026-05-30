# physiological-signal-pipeline
Python-based multimodal physiological signal processing pipeline for GSR and heart rate analysis in human neuroscience experiments.
# Physiological Signal Analysis Pipeline

This repository contains a Python script for preprocessing and analyzing multimodal physiological signals collected in human neuroscience experiments.

## Description

The script processes raw physiological data in BrainVision format and extracts features from:

* Galvanic Skin Response (GSR)
* Blood Volume Pulse (PPG / heart rate)

## Methods

The analysis pipeline includes:

* Signal resampling (50 Hz)
* Bandpass and low-pass filtering
* Decomposition of electrodermal activity using NeuroKit2 (cvxEDA method)
* Extraction of SCR events and tonic/phasic components
* Heart rate and HRV analysis (RMSSD, pNN50)

## Tools Used

* MNE-Python
* NeuroKit2
* NumPy
* Pandas

## Output

The script generates a CSV file containing participant-level physiological features:

* SCR count
* Mean tonic and phasic activity
* Mean heart rate
* HRV metrics (RMSSD, pNN50)

## Purpose

This pipeline was developed as part of experimental affective neuroscience research focusing on autonomic physiological responses during emotion-related experimental paradigms.

## Author

Zeynep Ş. Bayraktar
