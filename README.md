# PPE Detection Model Comparison Using YOLOv8

## Overview

This project evaluates and compares multiple pre-trained YOLOv8-based Personal Protective Equipment (PPE) detection models on a common test dataset.

The objective is to identify the most suitable model for detecting critical PPE components:

- Helmet / Hardhat
- Gloves
- Safety Vest

The comparison is performed on a labeled test dataset containing real-world construction and industrial safety images.

---

## Dataset

The evaluation dataset is in YOLO format and contains the following PPE-related classes:

| Class ID | Class Name |
|-----------|------------|
| 1 | Gloves |
| 3 | Helmet |
| 9 | Vest |

Only these three classes were considered during evaluation.

---

## Models Evaluated

### Model 1
Classes:
- Gloves
- Vest
- Goggles
- Helmet
- Mask
- Safety Shoe

### Model 2
Classes:
- Gloves
- Hardhat
- Safety Vest
- Additional PPE classes

### Model 3
Classes:
- Gloves
- Hardhat
- Safety Vest
- Additional PPE classes

To ensure fair comparison, equivalent class names were mapped as follows:

| Canonical Class | Model Class |
|----------------|------------|
| Helmet | Helmet / Hardhat |
| Gloves | Gloves |
| Vest | Vest / Safety Vest |

---

## Evaluation Metrics

The following metrics were used:

- True Positives (TP)
- False Positives (FP)
- False Negatives (FN)
- Precision
- Recall
- F1 Score

The final ranking was based on the Macro F1 Score across:

- Helmet
- Gloves
- Vest

---

## Project Structure

<img width="329" height="406" alt="image" src="https://github.com/user-attachments/assets/cfdb053f-d1e1-4ad2-aaec-993f7d01985b" />


---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/PPE-Model-Comparison.git
cd PPE-Model-Comparison
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Evaluation

Run the evaluation script:

```bash
python evaluate_models.py
```

The script evaluates all models on the same test dataset and generates performance metrics.

---

## Results

Each model is evaluated on the same set of labeled PPE images.

Generated outputs include:

- Precision
- Recall
- F1 Score
- Model Ranking
- Prediction Visualizations

<img width="222" height="152" alt="image" src="https://github.com/user-attachments/assets/7ffe411b-9638-4c50-a5a9-7cc811787256" />


---

## Model Weights

Due to GitHub file size limitations, model weights are not included in this repository.

Download model weights from:

https://drive.google.com/drive/folders/14gawDqO5zDvGf7WGawI00fqMChhTXrq3?usp=sharing

---

## Applications

This project can be applied to:

- Construction Site Safety Monitoring
- PPE Compliance Verification
- Industrial Worker Safety Inspection
- Automated Workplace Monitoring
- Real-Time CCTV Safety Analytics

---

## Technologies Used

- Python
- YOLOv8
- Ultralytics
- OpenCV
- Pandas
- NumPy
- Matplotlib

---

## Author

Internship Project

PPE Detection Model Evaluation and Comparison using YOLOv8
