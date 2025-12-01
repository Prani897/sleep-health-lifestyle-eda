# Sleep Health and Lifestyle - Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)
![Status](https://img.shields.io/badge/Status-Complete-success)
![License](https://img.shields.io/badge/License-MIT-green)

**Course:** CS696A - Full-Stack Enterprise Application Development  
**Institution:** Pace University  
**Team:** Group 3  
**Date:** December 2024

---

## 📊 Project Overview

This project performs comprehensive Exploratory Data Analysis (EDA) on the Sleep Health and Lifestyle dataset to understand factors affecting sleep quality and identify patterns in sleep disorders, lifestyle habits, and health metrics.

### 🎯 Objectives
- Analyze sleep patterns and quality across demographics
- Identify relationships between lifestyle factors and sleep
- Examine health metrics and their correlations
- Provide insights and recommendations for better sleep health

---

## 📁 Repository Structure
```
sleep-health-lifestyle-eda/
├── notebooks/
│   └── Sleep_Health_EDA_Complete.ipynb    # Main analysis notebook
├── data/
│   ├── sleep_health_dataset.csv           # Original dataset
│   └── processed datasets                 # Cleaned data
├── visualizations/                         # Generated plots
├── reports/                                # Final deliverables
├── README.md                              # This file
└── requirements.txt                       # Python dependencies
```

---

## 📊 Dataset Information

**Source:** [Kaggle - Sleep Health and Lifestyle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)

**Size:** 374 records × 13 features

**Features:**
- Demographics: Gender, Age, Occupation
- Sleep Metrics: Duration, Quality, Disorders
- Lifestyle: Physical Activity, Stress Level, Daily Steps
- Health: BMI Category, Blood Pressure, Heart Rate

---

## 🔍 Key Findings

### Sleep Patterns
- Average sleep duration: **~7.1 hours**
- Average sleep quality: **7-8/10**
- **40-45%** of individuals have sleep disorders
- Only **60-70%** get adequate sleep (7-9 hours)

### Correlations
- **Positive** correlation between sleep duration and quality
- **Negative** correlation between stress and sleep quality
- Physical activity inversely related to stress levels

### Health Insights
- Sleep disorders significantly impact sleep quality
- BMI category shows relationships with health metrics
- Age group influences sleep patterns

---

## 🚀 Getting Started

### Prerequisites
```bash
Python 3.8+
pandas
numpy
matplotlib
seaborn
scikit-learn
jupyter
```

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/YOUR-USERNAME/sleep-health-lifestyle-eda.git
cd sleep-health-lifestyle-eda
```

2. **Install dependencies:**
```bash
pip install -r requirements.txt
```

3. **Run the notebook:**
   - Open Google Colab: [Open in Colab](https://colab.research.google.com/github/YOUR-USERNAME/sleep-health-lifestyle-eda/blob/main/notebooks/Sleep_Health_EDA_Complete.ipynb)
   - Or use Jupyter: `jupyter notebook notebooks/Sleep_Health_EDA_Complete.ipynb`

---

## 📊 Visualizations

The analysis includes 15+ professional visualizations:
- Distribution plots for all key variables
- Categorical analysis (gender, disorders, BMI)
- Correlation heatmap
- Boxplots for group comparisons
- Scatter plots with regression lines

---

## 📈 Analysis Workflow

1. **Data Loading** - Import dataset from Google Drive
2. **Data Cleaning** - Handle missing values, remove duplicates
3. **Feature Engineering** - Create new categorical features
4. **Exploratory Analysis** - Generate visualizations and statistics
5. **Correlation Analysis** - Identify relationships between variables
6. **Insights Generation** - Summarize key findings

---

## 👥 Team Contributions

- **Person 1:** Sleep patterns and quality analysis
- **Person 2:** Lifestyle factors analysis
- **Person 3:** Health metrics analysis
- **Person 4:** Correlations and integration

---

## 📝 Results Summary

Our analysis revealed:
1. Significant positive correlation between sleep duration and quality
2. Stress negatively impacts sleep quality
3. Sleep disorders affect nearly half of the population
4. Physical activity is associated with lower stress levels
5. Age and occupation influence sleep patterns

### Recommendations
- Aim for 7-9 hours of sleep per night
- Increase physical activity to reduce stress
- Seek medical consultation for sleep disorders
- Maintain healthy BMI for better overall health

---

## 📚 References

1. [Sleep Health and Lifestyle Dataset - Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)
2. [CDC - Sleep and Sleep Disorders](https://www.cdc.gov/sleep/)
3. [WHO - Sleep Guidelines](https://www.who.int/)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🤝 Acknowledgments

- **Course Instructor:** CS696A - Pace University
- **Dataset Source:** Laksika Tharmalingam (Kaggle)
- **Tools:** Google Colab, Python, Pandas, Matplotlib, Seaborn

---

## 📧 Contact

**Nikunj**  
Pace University  
CS696A - Group 3

**Project Link:** [https://github.com/YOUR-USERNAME/sleep-health-lifestyle-eda](https://github.com/YOUR-USERNAME/sleep-health-lifestyle-eda)

---

⭐ **If you find this project helpful, please give it a star!**
```

4. **Update:**
   - Replace `YOUR-USERNAME` with your actual GitHub username
   - Update contact info

5. Click **"Commit changes"**

---

## 📦 **PART 6: Add Requirements.txt**

### **Step 6: Create Requirements File**

1. Click **"Add file"** → **"Create new file"**

2. **Filename:** `requirements.txt`

3. **Content:**
```
pandas==1.5.3
numpy==1.24.3
matplotlib==3.7.1
seaborn==0.12.2
scikit-learn==1.2.2
jupyter==1.0.0
```

4. Click **"Commit new file"**

---

## 📤 **PART 7: Upload Your Dataset and Visualizations**

### **Step 7: Upload Files via GitHub Web Interface**

**Option A: Web Upload (Easiest)**

1. Go to the `data` folder in your repository
2. Click **"Add file"** → **"Upload files"**
3. Drag and drop your CSV files:
   - `sleep_health_dataset.csv`
   - `sleep_health_processed.csv`
   - All person-specific CSVs
4. Commit message: `Add dataset files`
5. Click **"Commit changes"**

**Repeat for visualizations:**
1. Go to `visualizations` folder
2. Upload all your saved plot images (PNG/JPG)
3. Commit message: `Add analysis visualizations`

**Note:** GitHub has file size limits (25MB for web upload, 100MB total)

---

## 🔗 **PART 8: Add Colab Badge to Notebook**

### **Step 8: Make Notebook Easy to Open**

Your notebook already has the Colab link! When you saved from Colab with "Include a link to Colaboratory" checked, it automatically added the badge.

**Users can click the badge to open directly in Colab!**

---

## ✨ **PART 9: Make Repository Look Professional**

### **Step 9: Add Final Touches**

1. **Add Topics/Tags:**
   - Click the **gear icon** next to "About" (right side)
   - Add topics: `data-analysis`, `eda`, `python`, `sleep-health`, `data-science`, `visualization`
   - Add description: "EDA of Sleep Health & Lifestyle Dataset"
   - Save

2. **Add a License** (if you didn't earlier):
   - Click **"Add file"** → **"Create new file"**
   - Name it: `LICENSE`
   - Click **"Choose a license template"**
   - Select **"MIT License"**
   - Fill in year and name
   - Commit

3. **Create a .gitignore:**
   - Click **"Add file"** → **"Create new file"**
   - Name: `.gitignore`
   - Content:
```
   # Python
   __pycache__/
   *.py[cod]
   *$py.class
   *.so
   .Python
   
   # Jupyter Notebook
   .ipynb_checkpoints
   
   # Data files
   *.csv
   !sleep_health_dataset.csv
   
   # Virtual Environment
   venv/
   env/
   
   # OS
   .DS_Store
   Thumbs.db
```
   - Commit

---

## 🎓 **PART 10: Share Your Repository**

### **Step 10: Get Your Repository Link**

**Your repository URL is:**
```
https://github.com/YOUR-USERNAME/sleep-health-lifestyle-eda
```

### **Share with:**

**1. Your Team:**
```
Hey team! 

Our project is now on GitHub:
https://github.com/YOUR-USERNAME/sleep-health-lifestyle-eda

You can:
- View the complete analysis
- Download the notebook
- Open directly in Colab (click the badge)
- Clone the repository

Let me know if you need access!
```

**2. Your Professor:**
```
Dear Professor,

Our Group 3 project repository:
https://github.com/YOUR-USERNAME/sleep-health-lifestyle-eda

All code, analysis, and documentation are included.
The notebook can be opened directly in Google Colab via the badge.

Best regards,
Nikunj
```

**3. On Your Resume/LinkedIn:**
```
Sleep Health & Lifestyle Analysis
- Performed EDA on 374 records using Python (pandas, matplotlib, seaborn)
- Generated 15+ visualizations analyzing sleep patterns and health correlations
- Identified key factors affecting sleep quality through statistical analysis
- GitHub: https://github.com/YOUR-USERNAME/sleep-health-lifestyle-eda
