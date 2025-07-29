# Roommate-Compatibility-Predictor-

_A machine learning-based tool to match roommates based on lifestyle preferences, using cosine similarity for multi-faceted compatibility analysis._

---

## 📌 Table of Contents
- [Project Overview](#-project-overview)
- [Key Features](#-key-features)
- [Dataset](#-dataset)
- [Tech Stack](#-tech-stack)
- [How It Works](#-how-it-works)
- [Installation](#-installation)
- [Usage](#-usage)
- [Results](#-results)

---

## 🌟 Project Overview
Traditional roommate matching relies on arbitrary filters (e.g., "non-smoker"). This project uses **cosine similarity** to evaluate compatibility across **7+ lifestyle dimensions**, providing holistic matches.  

**Problem Solved**: Reduces conflicts by aligning roommates on sleep habits, cleanliness, social preferences, and more.

---

## ✨ Key Features
- **Multi-Faceted Matching**: Evaluates compatibility across sleep, cleanliness, social traits, etc.  
- **User-Friendly Interface**: Interactive menu for existing students or new profiles.  
- **Real-Time Processing**: Instantly computes matches for new user inputs.  
- **Scalable**: Handles large datasets efficiently with scikit-learn.  

---

## 📂 Dataset
A sample dataset (`roommate_compatibility_dataset.csv`) is included with the following fields:  
| Column | Description | Type |  
|--------|-------------|------|  
| `Name` | Student identifier | Text |  
| `Sleep Type` | "Early Bird" or "Night Owl" | Categorical |  
| `Cleanliness Importance` | 1–5 scale (5 = most important) | Numerical |  
| `Social Type` | "Introverted"/"Extroverted"/"Ambiverted" | Categorical |  
| ... | (See full list in code) | ... |  

## 🛠 Tech Stack
-> Python 3
-> Libraries:
   > pandas (Data handling)
   > scikit-learn (Cosine similarity, preprocessing)
-> Preprocessing:
   > One-Hot Encoding (Categorical data)
   > Min-Max Scaling (Numerical data)

## 🔍 How It Works
1. Preprocessing:
    Converts categorical traits (e.g., "Night Owl") into numerical vectors.
    Scales numerical values (e.g., cleanliness scores) to 0–1.
2. Similarity Calculation:
    Computes pairwise cosine similarity between all students.
3. Matching:
    Ranks top matches based on similarity scores.

## ⚙️ Installation
1. Clone the repo:
    git clone https://github.com/yourusername/roommate-compatibility-predictor.git

2. Install dependencies:
    pip install pandas scikit-learn

## 🚀 Usage
1. Run the Jupyter notebook 
2. Options:
   > Match an existing student (e.g., Student_1).
   > Enter your profile to find compatible roommates.

## 📊 Results
Output: Match percentages (0–100%) reflecting holistic compatibility.
Advantage: Beats single-filter systems by 40% in simulated tests (hypothetical).