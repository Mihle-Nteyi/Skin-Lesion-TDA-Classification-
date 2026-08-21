# Skin Lesion Classification using Topological Data Analysis

## Overview
This research project applies **Persistent Homology**, a core method in Topological Data Analysis (TDA), to classify skin lesions as benign or melanoma based on their topological features. 

Traditional image classification relies on shape and colour, but TDA captures **hidden structural patterns** that are invisible to the naked eye. This project demonstrates that melanoma lesions exhibit distinct topological signatures that persist across longer filtration scales compared to benign cases.

---

## Key Findings
- Melanoma lesions show **topological features (loops and voids)** that persist significantly longer in the filtration process than benign lesions
- Persistent homology captures the **increased structural complexity and irregularity** of malignant melanomas
- Successfully validated the computational pipeline on synthetic "circle cloud" data, detecting **1-dimensional cycles** with high accuracy
- Results suggest topological methods could improve **automated diagnostic support systems** for dermatology

---

## Thesis Abstract
> Topological Data Analysis (TDA) offers a powerful framework for analysing the shape and structure of complex datasets beyond traditional statistical measures. This project explores the application of persistent homology, a core methodology in TDA, to classify skin lesions from image data. We first validated our computational pipeline on synthetic "circle cloud" data, successfully demonstrating the ability of persistent homology to detect and quantify robust topological features, specifically 1-dimensional cycles. Subsequently, we applied this method to a dataset of clinical images comprising benign lesions and melanomas. Our analysis reveals that melanoma lesions exhibit topological features, namely loops and voids that persist across significantly longer scales in the filtration process compared to benign cases. These findings suggest that the increased structural complexity and irregularity of malignant melanomas are captured effectively by their persistent homology. We conclude that topological methods provide a novel and powerful quantitative descriptor for characterizing skin lesion morphology, with promising potential for improving automated diagnostic support systems.

---

## Methodology

### 1. Data Preprocessing
- Convert clinical images to grayscale
- Resize and normalise images for consistent analysis
- Extract point cloud data from images

### 2. Filtration
- Apply **Vietoris-Rips** and **Čech filtrations** to build simplicial complexes
- Track topological features across varying scales

### 3. Persistent Homology Computation
- Compute birth and death times for topological features (H₀, H₁, H₂)
- Use **Ripser**, **GUDHI**, and **Scikit-TDA** libraries

### 4. Visualisation
- Generate **persistence diagrams** and **barcodes**
- Compare topological signatures of benign vs melanoma lesions

### 5. Analysis
- Interpret persistence pairs and identify distinguishing features
- Quantify differences using **Bottleneck distance** and **Stability Theorem**

---

## Technologies Used

### Programming & Analysis
- **Python**: Core programming language
- **NumPy**: Numerical computing
- **Pandas**: Data manipulation
- **Matplotlib**: Data visualisation

### Topological Data Analysis
- **Ripser**: Fast Vietoris-Rips persistence computation
- **GUDHI**: Comprehensive TDA library (simplicial complexes, persistent homology)
- **Scikit-TDA**: Scikit-learn-style interface for TDA
- **Persim**: Persistence diagram visualisation and metrics

### Image Processing
- **Pillow (PIL)**: Image loading and preprocessing

### Environment
- **Google Colab**: Development and experimentation

---

## Repository Structure

## How to Run

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/skin-lesion-tda-classification.git
cd skin-lesion-tda-classification

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the analysis

Open notebooks/tda_skin_lesion_analysis.ipynb in Google Colab or Jupyter Notebook.

4. Upload images

Use the upload_images() function to load your own skin lesion images.

5. View results

Persistence diagrams and barcodes will be saved to the results/ directory.

---

Results

[You can add a screenshot of your persistence diagram here]

```
[Placeholder for persistence diagram]
```

What the diagram shows:

· Features far from the diagonal represent significant topological structures
· H₁ features (loops) that persist across long scales indicate structural complexity
· Melanoma lesions show more persistent H₁ features than benign lesions

---

Future Work

· Extend analysis to larger datasets with more lesion types
· Combine TDA with deep learning (convolutional neural networks)
· Build a user-friendly web application for dermatologists
· Integrate with clinical diagnostic workflows

---

Author

Mihle Nteyi

· 📧 Email: mihlenteyi.g@gmail.com
· 📱 Phone: 0614929689
· 📍 Location: Durban, South Africa
· 🔗 LinkedIn: [Your LinkedIn URL]
· 🐙 GitHub: github.com/yourusername

---

Supervisor

Dr Cerene Rathilal and Prof. K.J. Duffy
School of Mathematics
University of KwaZulu-Natal

---

License

This project is for research and educational purposes. For commercial use, please contact the author.

---

Acknowledgements

This research was conducted at the University of KwaZulu-Natal, School of Mathematics. Special thanks to my supervisors for their guidance and support throughout this project.

---

"Uncovering Hidden Structures: A Study of Persistent Homology in Topological Data Analysis"

```

---

