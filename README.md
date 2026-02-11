# Qstar-

---

# Personalized Healthcare Management using Reinforcement Learning

![Python](https://img.shields.io/badge/python-3.8%2B-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-2.0%2B-orange)
![Stable-Baselines3](https://img.shields.io/badge/stable--baselines3-latest-green)

An advanced personalized healthcare management system that leverages Reinforcement Learning (RL) with Proximal Policy Optimization (PPO) for accurate medical diagnosis and treatment recommendations.

---

## 🚀 Key Features

- **Intelligent Disease Diagnosis**: Analyzes symptoms with state-of-the-art ML models.
- **Personalized Treatment Plans**: Recommends tailored treatments based on patient data.
- **Medication Matching**: Uses cosine similarity for precise drug recommendations.
- **Precaution Guidance**: Suggests relevant precautions for diagnosed conditions.
- **Detailed Reports**: Generates comprehensive timestamped reports.
- **Continuous Learning**: Enhances recommendations through reinforcement learning.

---

## 📋 Requirements

- **Python 3.8+**
- **PyTorch**
- **Stable-Baselines3**
- **Pandas, NumPy, Scikit-learn, NLTK, Gym**

---

## 🔧 Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ishajangid/Qstar-
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Download NLTK data**:
   ```python
   import nltk
   nltk.download('punkt')
   ```

4. **Prepare your datasets**:
   - `Training.csv`: Disease training data
   - `medications.csv`: Medication data
   - `precautions_df.csv`: Precautions data
   - `medicine.csv`: Medicine details

---

## 💻 Usage

### Initialize and Run Diagnosis

```python
from diagnosis_system import AdvancedDiagnosisSystem


system = AdvancedDiagnosisSystem(
    disease_data_path='Training.csv',
    medication_data_path='medications.csv',
    precaution_data_path='precautions_df.csv',
    medicine_data_path='medicine.csv'
)


symptoms = "fever, headache, fatigue"
system.process_input(symptoms)
```

### Sample Output

```
======= Disease Diagnosis and Treatment Report =======
Date: 2024-10-26 07:11:43

Input Symptoms: fever, headache, fatigue

Top Predicted Disease: Fungal infection (Probability: 99.77%)
Other Possible Diseases:
- Impetigo: 0.11%
- Urinary tract infection: 0.06%
- Acne: 0.02%
- Heart attack: 0.01%

Recommended Medications: 
- Antifungal Cream, Fluconazole, Terbinafine, Clotrimazole, Ketoconazole

Precautions:
- Bath twice, use Dettol or neem in bathing water, keep area dry, use clean cloths

Additional Drug Recommendations:
- Zole IT 100mg Capsule 7'S: 0.5305
- Voraze 200mg Tablet 4'S: 0.5305
...
=====================================================
Note: Review by a healthcare professional is recommended.
```

---

## 🏗 Project Structure

```
medicine-recommending-system/
├── model_A.ipynb
├── model_B.ipynb
├── model_combined.ipynb
└── model_extra.ipynb
```

---

## 🔬 Technical Overview

### Reinforcement Learning

Utilizes PPO with:
- **State Space**: Patient symptoms and vital signs
- **Action Space**: Treatment recommendations
- **Reward Function**: Based on patient recovery
- **Policy Network**: Multi-Layer Perceptron (MLP)

### ICDIF Vector Implementation

ICDIF vectors encode disease information, including:
- Severity, Treatment Complexity, Recovery Patterns, Risk Factors

### Medication Matching

Applies cosine similarity to suggest medications:
```python
similarity_score = cosine_similarity(patient_vector, medication_vector)
```

---

## 📈 Performance

- **Improves** over traditional rule-based systems
- **Real-time** learning from patient responses
- **Continuous** adaptation and optimization

---

## 🎯 Future Directions

- **EHR Integration**
- **Vital Monitoring**
- **Mobile App Development**
- **Multi-language Support**
- **Enhanced Privacy**
- **Hospital System Compatibility**

---

## ✍️ Contributors

- Arpita
- Dhruv Bhalodia
- Daivik Hirpara
- Isha Jangir  
*(IIIT Vadodara - International Campus Diu)*

---
