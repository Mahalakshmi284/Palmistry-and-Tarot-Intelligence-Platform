# Dataset EDA Summary

## Overview

Exploratory Data Analysis (EDA) was performed on the two datasets used in the AI-Powered Palm & Tarot Intelligence Platform. The analysis was carried out using Python in Google Colab to understand the structure, features, data quality, and distributions of the available data.

## 1. Hand Images Dataset

The hand image dataset was obtained from Kaggle and contains palm and dorsal hand images, including left and right hands. The dataset also includes a `HandInfo.csv` metadata file.

### Metadata Features

* ID
* Age
* Gender
* Skin Color
* Accessories
* Nail Polish
* Aspect of Hand
* Image Name
* Irregularities

### EDA Performed

The following analyses were performed:

* Loaded the metadata using Pandas.
* Examined the first records using `head()`.
* Checked dataset dimensions using `shape`.
* Examined column names and data types.
* Checked for missing values.
* Generated statistical summaries.
* Analyzed the distribution of:

  * Gender
  * Age
  * Skin Color
  * Accessories
  * Nail Polish
  * Aspect of Hand
* Displayed random sample images to visually inspect image quality.

The dataset was selected because it provides a large collection of hand images with organized metadata and can be used for image analysis and MediaPipe-based hand landmark extraction.

## 2. Tarot Dataset

The tarot dataset was obtained from Kaggle and provided in JSON format.

### Available Information

* Card Name
* Arcana
* Suit
* Keywords
* Upright Meaning
* Reversed Meaning

### EDA Performed

The following analyses were performed:

* Loaded the JSON dataset using Python.
* Converted the JSON data into a structured DataFrame.
* Examined the dataset structure, shape, and columns.
* Checked data types and missing values.
* Generated statistical summaries.
* Analyzed:

  * Major vs Minor Arcana distribution
  * Suit distribution
  * Word frequency
  * Meaning length

## EDA Outcome

The EDA provided an understanding of the available image metadata and tarot information, along with the overall structure and data quality of both datasets.

This analysis establishes the foundation for the next stages of the project:

```text
Dataset
   ↓
EDA ✅
   ↓
Preprocessing
   ↓
MediaPipe
   ↓
YOLO Training
   ↓
Model Evaluation
   ↓
Palm Analysis Engine
```
