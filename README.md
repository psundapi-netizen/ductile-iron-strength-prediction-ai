# **Prediction of Ultimate Tensile Strength of Ductile Iron by Artificial Intelligence**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](INSERT_YOUR_COLAB_LINK_HERE)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

<div align="center">

**Tharika Puntlert (ธาริกา พันธุ์เลิศ)** *(Published under the name “Dharika Phanlert” in the journal record)* Department of Materials and Metallurgical Engineering  
**Suranaree University of Technology (SUT)**, Nakhon Ratchasima, Thailand

📄 *Science and Engineering Connect*, Vol. 47, No. 3 (2024), pp. 244–256  
📘 ISSN 3027-7914 (Online)  
🔗 [Full Paper on TCI-ThaijO](https://ph04.tci-thaijo.org/index.php/SEC/article/view/7699)

</div>

---

## **Abstract**
This research investigates the application of **Artificial Intelligence (AI)** to predict the **Ultimate Tensile Strength (UTS)** of ductile iron based on its chemical composition. Two machine learning algorithms — **Multi-linear Regression (MLR)** and **Multi-layer Perceptron (MLP)** — were employed to evaluate predictive performance. The study aims to develop a data-driven approach for predicting mechanical properties prior to casting, reducing the need for destructive testing and enabling better quality control.

---

## **⚠️ Note on Repository Data**
> **Important:** Due to the proprietary nature of the industrial data used in the original publication, the code in this repository utilizes **Synthetic Data** generated based on the statistical distribution and ranges specified in the paper.
> * **Purpose:** To demonstrate the coding implementation, model architecture, and data processing pipeline.
> * **Data Logic:** The synthetic data mimics the relationships found in the study (e.g., Carbon's effect on strength) but does not represent specific confidential samples.

---

## **1. Introduction**
The tensile strength of ductile iron is influenced by multiple alloying elements. Conventional testing requires destructive experiments which are costly and time-consuming. This study introduces an AI-based model to estimate tensile strength using only chemical composition data, enabling early-stage prediction for manufacturing quality control.

---

## **2. Dataset Details (Original Study)**
The findings in the published paper are based on actual experimental data with the following characteristics:

| Parameter | Description |
|------------|-------------|
| **Samples** | 55 (collected from academic sources and experiments) |
| **Input Variables (6)** | Carbon (C), Silicon (Si), Manganese (Mn), Sulfur (S), Magnesium (Mg), Copper (Cu) |
| **Output Variable** | Ultimate Tensile Strength (MPa) |
| **Data Split** | 80% Training : 20% Testing |

---

## **3. Methodology**

| Step | Description |
|------|--------------|
| **Data Processing** | Cleaning, normalization (StandardScaler), and correlation analysis. |
| **Modeling Techniques** | **Multi-linear Regression (MLR):** Used as a baseline.<br>**Multi-layer Perceptron (MLP):** A neural network optimized with 1 hidden layer (100 neurons), ReLU activation, and Adam solver. |
| **Evaluation Metrics** | Mean Absolute Error (MAE) |
| **Validation** | Comparison between models and parameter influence study. |

---

## **4. Results and Discussion (From Published Paper)**
The following results demonstrate the performance of the models on the actual validation dataset:

| Model | Mean Absolute Error (MAE) | Remarks |
|--------|----------------------------|----------|
| Multi-linear Regression | ~25 MPa | Baseline result indicating linear trends. |
| Multi-layer Perceptron | **~16 MPa** | **Best-performing model.** Capable of capturing non-linear relationships. |

**Key Findings:**
* **Carbon and Silicon** content are the most influential factors affecting tensile strength.
* The **Manganese–Copper–Silicon** interaction significantly affects UTS prediction.
* The MLP model achieved high accuracy with an MAE well below the **50 MPa** standard threshold for grade classification.

---

## **5. 🚀 Live Demo & Usage**
You can run the simulation model directly in your browser to see the code in action:

1.  Click the **"Open in Colab"** badge at the top of this page.
2.  Run the notebook cells to generate synthetic data.
3.  Observe the training process of MLR and MLP models.
4.  View the visualization comparing Predicted vs. Synthetic Actual values.

---

## **6. Tools and Technologies**
* **Language:** Python
* **IDE:** PyCharm (Original Research), Google Colab (Demo)
* **Libraries:**
    * `scikit-learn` (Model building)
    * `pandas`, `numpy` (Data manipulation)
    * `matplotlib`, `seaborn` (Visualization)

---

## **7. Conclusion**
The research demonstrates that **machine learning techniques** can effectively predict the **ultimate tensile strength** of ductile iron using its **chemical composition** alone. This contributes to the development of **intelligent quality control systems** for metal casting industries, aligning with Industry 4.0 goals.

---

## **Authors**
W. Thongking, R. Sinthusing, **D. Phanlert (Tharika Puntlert)**, Y. Noimueang, U. Kitkumthorn, P. Mitsomwang, R. Borrisutthekul*

---

## **Publication Timeline**
| Stage | Date |
|--------|------|
| Received | October 2023 |
| Revised | June 2024 |
| Accepted | August 2024 |

---

## **Keywords**
*Machine Learning • Artificial Intelligence • Ductile Iron • Tensile Strength Prediction • Materials Science*

---

<div align="center">

**© 2024 Tharika Puntlert.** *This repository serves as a portfolio demonstration of the research published in Science and Engineering Connect.*

</div>
