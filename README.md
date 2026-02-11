# 🏥 Personalized Healthcare Management System using Reinforcement Learning

An AI-powered healthcare management system that predicts diseases from symptoms and recommends personalized treatments using Reinforcement Learning (PPO).

Built with Python, PyTorch, and Stable-Baselines3.

---

## 🚀 Features

- 🔍 Disease prediction from symptoms
- 💊 Personalized medication recommendations
- ⚠️ Precaution suggestions
- 📄 Automated diagnosis report generation
- 🤖 Reinforcement Learning for continuous improvement

---

## 🛠 Tech Stack

- Python 3.8+
- PyTorch
- Stable-Baselines3
- Pandas
- NumPy
- Scikit-learn
- NLTK
- OpenAI Gym

---

## 📦 Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Download NLTK Data

```python
import nltk
nltk.download('punkt')
```

---

## 📂 Required Dataset Files

Place the following dataset files in the root directory:

- `Training.csv`
- `medications.csv`
- `precautions_df.csv`
- `medicine.csv`

---

## ▶️ Usage

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

---

## 🧠 How It Works

### Disease Prediction
A trained machine learning model analyzes symptoms and predicts the most probable disease.

### Medication Recommendation
Cosine similarity is used to match patient condition vectors with medication vectors.

```python
similarity_score = cosine_similarity(patient_vector, medication_vector)
```

### Reinforcement Learning (PPO)

- **State** → Patient symptoms  
- **Action** → Treatment recommendation  
- **Reward** → Patient recovery outcome  
- **Policy** → Multi-layer perceptron (MLP)

The system continuously improves recommendations through interaction.

---

## 📊 Sample Output

```
======= Diagnosis Report =======

Input Symptoms: fever, headache, fatigue
Predicted Disease: Fungal infection
Probability: 99.77%

Recommended Medications:
- Fluconazole
- Terbinafine
- Clotrimazole

Precautions:
- Maintain hygiene
- Keep affected area dry

=================================
```

---

## 📁 Project Structure

```
medicine-recommending-system/
│
├── diagnosis_system.py
├── model_A.ipynb
├── model_B.ipynb
├── model_combined.ipynb
├── model_extra.ipynb
├── requirements.txt
└── README.md
```

---

## 🔮 Future Improvements

- Electronic Health Record (EHR) integration
- Real-time vital monitoring
- Mobile application support
- Multi-language support
- Enhanced privacy and security

---

## ⚠️ Disclaimer

This project is for educational and research purposes only.  
Always consult a certified healthcare professional before taking medical treatment.
