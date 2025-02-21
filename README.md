# Mangrove Health Prediction through Neuro-Fuzzy Inference #

## 📌 Overview  ##

This project presents an adaptive system built with Neuro-Fuzzy Inference to identify mangrove species and assess their health despite challenges such as spectral blending, changing environmental conditions, and limited labeled data.

The system integrates neural networks for pattern recognition and fuzzy logic for handling uncertainty. It classifies mangroves into three health clusters: Good, Moderate, and Poor, with an accuracy of 95.8%. The model leverages hyperspectral and multispectral data to extract key vegetation indices and chlorophyll absorption metrics for precise classification.

## 🌱 Steps  ##

✅ Species Identification: The leaves of the mangrove are classified into the three species of *Rhizophora apiculata*, *Avicennia officinalis*, and *Sonneratia alba* from a 
                           total of 240 images collected(100 - *Rhizophora apiculata*,70 - *Avicennia officinalis*,70 - *Sonneratia alba*). 

✅ Feature Extraction: Entropy, leaf vein texture analysis using Gabor filters, Green-to Red ratio statistics, Chlorophyll Absorption Index, Hue index, Fractal patterns, 
                        etc. are extracted from the images, to create the dataset as per the three leaf species. The final dataset had 241 instances and 29 attributes.

✅ Dimensionality Reduction: Using Principal Component Analysis (PCA) was performed to reduce the dimensionality of the dataset, identifying the top 11 features to be 
                             considered, contributing 60.52% variance of the dataset.

✅ Health Categorization: The tree leaves are then categorized as Good, Moderate, or Poor using Fuzzy clustering mechanism.

✅ Neuro-Fuzzy System: Combines fuzzy logic with neural networks for adaptive decision-making.


## 📊 Results ##

- Classification Accuracy: 95.8%

- Steady Health Recognition: 98.01%

  | Health Condition | No. of Instances |
  | ---------------- | ---------------- |
  | Good             | 65               |
  | Moderate         | 92               |
  | Poor             | 83               |

## 🔹 Fuzzy Rules Extracted ##

The model generated 9 fuzzy rules, explaining how different features influence health classification for each species.

# 🛠 Installation #

## Clone the repository
```bash
git clone https://github.com/arkaprabde/HealthFuzz.git
```
