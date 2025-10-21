# Interpretable Deep Learning with Fuzzy Inference for Medical Prognosis

## 📘 Overview
This project presents an interpretable deep learning framework for **medical prognosis**, combining the predictive accuracy of **Deep Neural Networks (DNN)** with the explainability of a **Fuzzy Inference System (FIS)**.  
Using the **Breast Cancer Wisconsin (Diagnostic)** dataset from the **UCI Machine Learning Repository**, the model predicts whether a tumor is benign or malignant and provides a human-understandable explanation for its decision.

The main objective is to develop a **trustworthy, interpretable AI system** that bridges the gap between data-driven accuracy and clinical transparency.

---

## 🧠 Abstract
Medical prognosis plays a key role in early diagnosis and personalized treatment planning. While deep learning models provide high predictive accuracy, their lack of interpretability limits clinical trust.  
This project introduces a hybrid system titled **“Interpretable Deep Learning with Fuzzy Inference for Medical Prognosis”**, integrating DNN for precise classification and FIS for transparent reasoning.  
The model achieved a test accuracy of **96.49%** using standardized breast cancer data and generated fuzzy-based linguistic outputs like *Good*, *Moderate*, or *Poor* prognosis. This dual approach improves clinical confidence by offering both accurate predictions and human-readable explanations.

---

## 🩺 Dataset
- **Dataset Name:** Breast Cancer Wisconsin (Diagnostic)
- **Source:** UCI Machine Learning Repository
- **Link:** https://archive.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic
- **Samples:** 569  
- **Attributes:** 30 quantitative features  
- **Classes:** Benign (0) and Malignant (1)

Each feature represents measurements derived from **fine needle aspirate (FNA)** images of breast tissue.

---

## ⚙️ Methodology

The proposed workflow consists of two main stages — **Deep Learning Model (DNN)** for accurate prediction and **Fuzzy Inference System (FIS)** for interpretability.

### 🔹 Data Preparation
1. **Data Cleaning:** Removed missing and duplicate records.  
2. **Label Encoding:** Converted categorical diagnostic outcomes to binary form.  
3. **Feature Scaling:** Applied StandardScaler to normalize data.  
4. **Data Splitting:** 80% for training and 20% for testing.

---

### 🧩 Model Architecture
#### Deep Learning Model (DNN)
- **Input Layer:** 30 features  
- **Hidden Layers:** 32 and 16 neurons (ReLU activation)  
- **Dropout:** 0.2  
- **Output Layer:** Sigmoid neuron for binary classification  
- **Optimizer:** Adam  
- **Loss Function:** Binary Cross-Entropy  
- **Epochs:** 50  

#### Fuzzy Inference System (FIS)
- **Features Used:** Mean Radius, Mean Texture  
- **Steps:**
  1. **Feature Selection**
  2. **Fuzzification**
  3. **Rule Formation**
  4. **Defuzzification**

---

## 🧾 Workflow Diagram

The complete methodology is shown in the workflow diagram below:

![Workflow of Proposed Model](/image.png)

*Figure: Workflow of the hybrid model integrating Deep Learning and Fuzzy Inference for medical prognosis.*

---

## 📊 Results and Performance

| Metric | Value |
|--------|--------|
| **Accuracy** | 96.49% |
| **Epochs** | 50 |
| **Optimizer** | Adam |
| **Loss Function** | Binary Cross-Entropy |

### Fuzzy Interpretation
- **Good Prognosis:** Small radius, smooth texture  
- **Moderate Prognosis:** Medium radius, normal texture  
- **Poor Prognosis:** Large radius, coarse texture  

Example:  
A sample with a malignant probability of 0.91 from DNN received a **fuzzy score of 7.6**, interpreted as *Moderate*.  

This hybrid output ensures that clinicians receive both numerical accuracy and linguistic interpretability.

---

## ⚠️ Limitations
1. **Dataset Size:** Only 569 samples; larger datasets could improve generalization.  
2. **Feature Scope:** Fuzzy system used only two features for clarity; future versions can include more.  
3. **Binary Classification:** Focused on benign vs malignant only.  
4. **Evaluation Metrics:** Accuracy used as the main metric; more detailed metrics (precision, recall, F1) can be added.  

---

## 🚀 Future Scope
- **Multi-disease Prediction:** Extend the model to handle multiple diseases.  
- **Feature Expansion:** Add more clinically relevant features to FIS.  
- **Real-Time Integration:** Deploy the model in hospital systems for live decision support.  
- **Advanced Explainability:** Combine fuzzy logic with visual tools such as SHAP or LIME.  
- **Cross-dataset Validation:** Evaluate across varied medical datasets for robustness.  

---

## 🧩 Tools and Technologies
- **Programming Language:** Python  
- **Libraries Used:** TensorFlow / Keras, Scikit-learn, NumPy, Matplotlib, Fuzzy Logic Toolbox  
- **Platform:** Jupyter Notebook  
- **Dataset Source:** UCI Machine Learning Repository  

---

## 🧑‍🔬 Key Contributions
- Developed a hybrid DNN–FIS framework for interpretable medical prognosis.  
- Achieved strong predictive accuracy with explainable fuzzy reasoning.  
- Demonstrated how AI can enhance trust and transparency in healthcare.  

---

## 📚 References
1. Chatterjee, P., Banerjee, S., & Saha, D. (2022). *Deep neural network ensemble for breast cancer diagnosis and prognosis using UCI datasets.* Biomedical Signal Processing & Control, 74, 103512.  
2. Zhang, R., Han, J., Li, J., & Zhao, Y. (2021). *Interpretable deep learning model for medical image analysis using SHAP and Grad-CAM.* IEEE Access, 9, 153215–153225.  
3. Hussain, S., & Khan, R. (2020). *A hybrid intelligent system for diabetes prediction using decision tree and fuzzy inference.* Journal of Intelligent & Fuzzy Systems, 38(5), 6393–6405.  
4. Ahmed, M., Paul, B., & Farhana, S. (2019). *A comparative analysis of machine learning algorithms for breast cancer prediction using the UCI dataset.* IJCA, 182(40), 22–29.  
5. Doi, K. (2018). *Computer-aided diagnosis in medical imaging: Historical review, current status, and future potential.* Computerized Medical Imaging and Graphics, 66(2), 1–10.  

---

## 📄 License
This project is licensed under the **MIT License**. You are free to use, modify, and distribute it with proper attribution.

---

## 👩‍💻 Authors
**Shivani Toorpu**  
Department of CSE(AI&ML) 
Vardhaman College of Engineering
toorpushivani@gmail.com

**Bitla Pavan**  
Department of CSE(AI&ML) 
Vardhaman College of Engineering
pavanbitla21@gmail.com

**Vandan Kumar**  
Department of CSE(AI&ML) 
Vardhaman College of Engineering
kvk22510@gmail.com

---

> *This project demonstrates that combining deep learning with fuzzy reasoning can produce medical AI systems that are not only accurate but also interpretable, reliable, and clinically meaningful.*

