# EEG-SignalProcessing-DeepLearning

## Project Overview

This project aims to classify EEG signals recorded before and during an arithmetic task. The dataset consists of EEG recordings from 36 individuals, with each recording having a rest (before task) and task (during arithmetic task) segment. The project involves exploratory data analysis (EDA), power spectral density (PSD) calculation across five frequency bands, and the development of two deep learning models, EEGNet and TSCeption, to differentiate between rest and task EEG signals.

## Table of Contents

	1.	Project Structure
	2.	Installation
	3.	Dataset
	4.	Exploratory Data Analysis (EDA)
	5.	Power Spectral Density (PSD) Calculation
	6.	Models
	•	EEGNet
	•	TSCeption
	7.	Results
	8.	Contributing
	9.	License

### Project Structure
```
├── README.md
├── requirements.txt
├── combined.ipynb
├── notebooks
     ├── eda.ipynb
     ├── psd.ipynb
     ├── eegnet-v1.ipynb
     ├── tsception.ipynb
```
### Installation

Clone the repository:

```bash
git clone https://github.com/Ayush-Singh677/EEG-SignalProcessing-DeepLearning.git
cd EEG-SignalProcessing-DeepLearning
```

Install the required packages:
```bash
pip install -r requirements.txt
```
### Dataset
The data is sourced from the Mental Arithmetic
Tasks Dataset available at PhysioNet (https://physionet.org/content/eegmat/1.0.0/). The
dataset is pre-cleaned and ready for use, allowing you to focus on model implementation
and evaluation.

### Exploratory Data Analysis (EDA)
EDA is performed to understand the distribution and characteristics of the EEG data. This includes visualizing the EEG signals and their statistical properties.

The EDA notebook is available at eda.ipynb.
    
### Power Spectral Density (PSD) Calculation
PSD is calculated for each EEG signal across five frequency bands: Delta, Theta, Alpha, Beta, and Gamma. This helps in understanding the power distribution across different frequency ranges.

The PSD calculation notebook is available at psd.ipynb.

### Models
EEGNet : EEGNet is a compact convolutional neural network designed specifically for EEG-based brain-computer interfaces. It is implemented in eegnet.py. 

TSCeption : TSCeption is a time-series-based model that captures temporal dependencies and patterns in the EEG data. It is implemented in tsception.py.

### Results
The performance metrics of the models are are accuracy, precision, recall, f1.

### Contributing

Contributions are welcome! 

### License

This project is licensed under the MIT License.
