# 🌙 Sleep Health and Lifestyle - Exploratory Data Analysis

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=for-the-badge&logo=python)
![Status](https://img.shields.io/badge/Status-Complete-success?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter)

**Course:** CS 661 – Python Programming  
**Institution:** Pace University  
**Team:** Group 3  
**Date:** Fall 2025

---

## 📋 Table of Contents
- [Project Overview](#-project-overview)
- [System Architecture](#-system-architecture)
- [Data Flow](#-data-flow)
- [Analysis Workflow](#-analysis-workflow)
- [Key Findings](#-key-findings)
- [Dataset Information](#-dataset-information)
- [Getting Started](#-getting-started)
- [Visualizations](#-visualizations)
- [Results](#-results)
- [Team](#-team-contributions)

---

## 📊 Project Overview

This project performs comprehensive Exploratory Data Analysis (EDA) on the Sleep Health and Lifestyle dataset to understand factors affecting sleep quality and identify patterns in sleep disorders, lifestyle habits, and health metrics.

### 🎯 Objectives
- 📈 Analyze sleep patterns and quality across demographics
- 🔗 Identify relationships between lifestyle factors and sleep
- 💊 Examine health metrics and their correlations
- 💡 Provide insights and recommendations for better sleep health

---

## 🏗️ System Architecture

```mermaid
graph TB
    subgraph "Data Sources"
        A[Kaggle Dataset] -->|CSV Download| B[Raw Data]
    end
    
    subgraph "Data Processing Pipeline"
        B --> C[Data Loading]
        C --> D[Data Cleaning]
        D --> E[Feature Engineering]
        E --> F[Data Validation]
    end
    
    subgraph "Analysis Layer"
        F --> G[Descriptive Statistics]
        F --> H[Correlation Analysis]
        F --> I[Categorical Analysis]
        F --> J[Health Metrics Analysis]
    end
    
    subgraph "Visualization Engine"
        G --> K[Distribution Plots]
        H --> L[Heatmaps]
        I --> M[Bar Charts & Count Plots]
        J --> N[Boxplots & Scatter Plots]
    end
    
    subgraph "Output & Reporting"
        K --> O[Jupyter Notebook]
        L --> O
        M --> O
        N --> O
        O --> P[GitHub Repository]
        O --> Q[Reports & Insights]
    end
    
    style A fill:#4ecdc4
    style B fill:#ff6b6b
    style F fill:#95e1d3
    style O fill:#f38181
    style P fill:#aa96da
```

---

## 🔄 Data Flow

```mermaid
sequenceDiagram
    participant User
    participant Notebook as Jupyter Notebook
    participant Data as Dataset
    participant Pandas as Pandas/NumPy
    participant Viz as Matplotlib/Seaborn
    participant Output as Results
    
    User->>Notebook: Run Analysis
    Notebook->>Data: Load CSV
    Data->>Pandas: Return Raw Data
    
    Pandas->>Pandas: Clean Data
    Pandas->>Pandas: Handle Missing Values
    Pandas->>Pandas: Feature Engineering
    
    Notebook->>Pandas: Request Statistics
    Pandas->>Output: Descriptive Stats
    
    Notebook->>Pandas: Request Correlations
    Pandas->>Viz: Generate Heatmap
    Viz->>Output: Correlation Matrix
    
    Notebook->>Pandas: Group Analysis
    Pandas->>Viz: Create Plots
    Viz->>Output: Visualizations
    
    Output->>User: Display Results
    Output->>User: Save to Files
```

---

## 🔬 Analysis Workflow

```mermaid
flowchart LR
    A[Start] --> B[Load Dataset]
    B --> C{Data Quality Check}
    C -->|Issues Found| D[Data Cleaning]
    C -->|Clean| E[Exploratory Analysis]
    D --> E
    
    E --> F[Univariate Analysis]
    E --> G[Bivariate Analysis]
    E --> H[Multivariate Analysis]
    
    F --> I[Generate Visualizations]
    G --> I
    H --> I
    
    I --> J[Statistical Testing]
    J --> K[Correlation Analysis]
    K --> L[Extract Insights]
    
    L --> M{More Analysis Needed?}
    M -->|Yes| E
    M -->|No| N[Generate Report]
    N --> O[Save Results]
    O --> P[End]
    
    style A fill:#4ecdc4
    style D fill:#ff6b6b
    style I fill:#95e1d3
    style L fill:#f38181
    style P fill:#aa96da
```

---

## 📁 Repository Structure

```mermaid
graph TD
    A[sleep-health-lifestyle-eda/] --> B[Sleep_Health_EDA_Complete.ipynb]
    A --> C[data/]
    A --> D[visualizations/]
    A --> E[reports/]
    A --> F[README.md]
    A --> G[LICENSE]
    A --> H[.gitignore]
    
    C --> C1[Sleep_health_and_lifestyle_dataset.csv]
    C --> C2[README.md]
    
    D --> D1[distribution_plots/]
    D --> D2[correlation_plots/]
    D --> D3[categorical_plots/]
    
    E --> E1[final_report.pdf]
    E --> E2[README.md]
    
    style A fill:#667eea
    style B fill:#764ba2
    style C fill:#f093fb
    style D fill:#4facfe
    style E fill:#43e97b
```

---

## 📊 Dataset Information

**Source:** [Kaggle - Sleep Health and Lifestyle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)

**Size:** 374 records × 13 features

### Features Overview

```mermaid
mindmap
  root((Sleep Health Dataset))
    Demographics
      Gender
      Age
      Occupation
    Sleep Metrics
      Duration
      Quality
      Sleep Disorders
    Lifestyle Factors
      Physical Activity Level
      Stress Level
      Daily Steps
    Health Indicators
      BMI Category
      Blood Pressure
      Heart Rate
```

---

## 🔍 Key Findings

### Sleep Patterns Insights

```mermaid
pie title Sleep Duration Distribution
    "Adequate Sleep (7-9h)" : 65
    "Insufficient Sleep (<7h)" : 20
    "Excessive Sleep (>9h)" : 15
```

### Health Correlations

```mermaid
graph LR
    A[Sleep Duration] -->|+0.88| B[Sleep Quality]
    C[Stress Level] -->|-0.90| B
    D[Physical Activity] -->|-0.75| C
    E[Age] -->|-0.12| A
    F[Sleep Disorder] -->|-0.56| B
    
    style A fill:#4ecdc4
    style B fill:#95e1d3
    style C fill:#ff6b6b
    style D fill:#4ecdc4
    style F fill:#ff6b6b
```

### Key Statistics
- **Average Sleep Duration:** ~7.1 hours
- **Average Sleep Quality:** 7-8/10
- **Population with Sleep Disorders:** 40-45%
- **Individuals with Adequate Sleep:** 60-70%

---

## 🚀 Getting Started

### Prerequisites
```bash
Python 3.8+
pandas >= 1.5.3
numpy >= 1.24.3
matplotlib >= 3.7.1
seaborn >= 0.12.2
scikit-learn >= 1.2.2
jupyter >= 1.0.0
```

### Installation

1. **Clone the repository:**
```bash
git clone https://github.com/Prani897/sleep-health-lifestyle-eda.git
cd sleep-health-lifestyle-eda
```

2. **Create virtual environment (optional but recommended):**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install dependencies:**
```bash
pip install -r requirements.txt
```

4. **Launch Jupyter Notebook:**
```bash
jupyter notebook Sleep_Health_EDA_Complete.ipynb
```

**Or open directly in Google Colab:**

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Prani897/sleep-health-lifestyle-eda/blob/main/Sleep_Health_EDA_Complete.ipynb)

---

## 📊 Visualizations

The analysis includes 15+ professional visualizations:

### Visualization Categories

```mermaid
graph TD
    A[EDA Visualizations] --> B[Distribution Analysis]
    A --> C[Categorical Analysis]
    A --> D[Correlation Analysis]
    A --> E[Comparative Analysis]
    
    B --> B1[Histograms]
    B --> B2[KDE Plots]
    B --> B3[Box Plots]
    
    C --> C1[Count Plots]
    C --> C2[Bar Charts]
    C --> C3[Pie Charts]
    
    D --> D1[Heatmap]
    D --> D2[Pair Plots]
    D --> D3[Scatter Plots]
    
    E --> E1[Group Comparisons]
    E --> E2[Trend Analysis]
    
    style A fill:#667eea
    style B fill:#f093fb
    style C fill:#4facfe
    style D fill:#43e97b
    style E fill:#fa709a
```

---

## 📈 Analysis Methodology

### Data Processing Pipeline

```mermaid
stateDiagram-v2
    [*] --> LoadData
    LoadData --> InspectData
    InspectData --> CleanData
    CleanData --> HandleMissing
    HandleMissing --> RemoveDuplicates
    RemoveDuplicates --> FeatureEngineering
    FeatureEngineering --> Validation
    Validation --> Analysis
    Analysis --> Visualization
    Visualization --> Insights
    Insights --> [*]
    
    note right of CleanData
        Remove null values
        Correct data types
        Handle outliers
    end note
    
    note right of FeatureEngineering
        Create age groups
        Categorize BMI
        Calculate derived metrics
    end note
```

---

## 📝 Results Summary

### Key Discoveries

1. **✅ Strong Positive Correlation:** Sleep duration and quality (r = +0.88)
2. **⚠️ Negative Impact:** Stress significantly reduces sleep quality (r = -0.90)
3. **📊 Prevalence:** Sleep disorders affect nearly half the population (40-45%)
4. **💪 Lifestyle Factor:** Physical activity correlates with lower stress levels
5. **👥 Demographics:** Age and occupation influence sleep patterns

### Recommendations

```mermaid
graph TD
    A[Sleep Health Recommendations] --> B[Sleep Duration]
    A --> C[Lifestyle Changes]
    A --> D[Medical Consultation]
    A --> E[Health Management]
    
    B --> B1[Aim for 7-9 hours nightly]
    B --> B2[Maintain consistent schedule]
    
    C --> C1[Increase physical activity]
    C --> C2[Reduce stress through exercise]
    C --> C3[Track daily steps target: 10,000]
    
    D --> D1[Seek help for sleep disorders]
    D --> D2[Regular health checkups]
    
    E --> E1[Maintain healthy BMI]
    E --> E2[Monitor blood pressure]
    E --> E3[Track heart rate]
    
    style A fill:#667eea
    style B fill:#4ecdc4
    style C fill:#95e1d3
    style D fill:#ff6b6b
    style E fill:#4facfe
```

---

## 👥 Team Contributions

**Group 3 Members:**

| Member | Contribution | Focus Area |
|--------|--------------|------------|
| **Person 1** | Sleep patterns analysis | Duration & Quality metrics |
| **Person 2** | Lifestyle factors | Physical activity & Stress |
| **Person 3** | Health metrics | BMI, BP, Heart rate |
| **Person 4** | Data integration | Correlations & insights |

---

## 🛠️ Technologies Used

```mermaid
graph LR
    A[Technologies] --> B[Languages]
    A --> C[Libraries]
    A --> D[Tools]
    A --> E[Platform]
    
    B --> B1[Python 3.8+]
    
    C --> C1[Pandas]
    C --> C2[NumPy]
    C --> C3[Matplotlib]
    C --> C4[Seaborn]
    C --> C5[Scikit-learn]
    
    D --> D1[Jupyter Notebook]
    D --> D2[Git/GitHub]
    D --> D3[Google Colab]
    
    E --> E1[Kaggle]
    E --> E2[VS Code]
    
    style A fill:#667eea
    style B1 fill:#3776ab
    style C1 fill:#150458
    style C3 fill:#11557c
    style D1 fill:#f37626
```

---

## 📚 References

1. [Sleep Health and Lifestyle Dataset - Kaggle](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)
2. [CDC - Sleep and Sleep Disorders](https://www.cdc.gov/sleep/)
3. [WHO - Sleep Guidelines](https://www.who.int/)
4. [National Sleep Foundation](https://www.sleepfoundation.org/)
5. [Python Data Science Handbook](https://jakevdp.github.io/PythonDataScienceHandbook/)

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 Prani897

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files.
```

---

## 🤝 Acknowledgments

- **Course Instructor:** CS661 - Pace University
- **Dataset Source:** Laksika Tharmalingam (Kaggle)
- **Tools:** Google Colab, Python, Pandas, Matplotlib, Seaborn
- **Team:** Group 3 Members for collaborative effort

---

## 📧 Contact

**Prani897**  
Pace University  
CS661 - Group 3

**GitHub:** [@Prani897](https://github.com/Prani897)  
**Project Link:** [https://github.com/Prani897/sleep-health-lifestyle-eda](https://github.com/Prani897/sleep-health-lifestyle-eda)

---

## 🌟 Project Stats

![GitHub stars](https://img.shields.io/github/stars/Prani897/sleep-health-lifestyle-eda?style=social)
![GitHub forks](https://img.shields.io/github/forks/Prani897/sleep-health-lifestyle-eda?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/Prani897/sleep-health-lifestyle-eda?style=social)

---

## 📈 Future Enhancements

```mermaid
graph TB
    A[Future Work] --> B[Machine Learning]
    A --> C[Additional Data]
    A --> D[Interactive Dashboard]
    A --> E[Mobile App]
    
    B --> B1[Predictive Models]
    B --> B2[Classification Algorithms]
    B --> B3[Clustering Analysis]
    
    C --> C1[Larger Dataset]
    C --> C2[Time-series Data]
    C --> C3[Wearable Device Data]
    
    D --> D1[Plotly Dash]
    D --> D2[Streamlit App]
    D --> D3[Real-time Analytics]
    
    E --> E1[Sleep Tracker]
    E --> E2[Recommendations Engine]
    
    style A fill:#667eea
    style B fill:#f093fb
    style C fill:#4facfe
    style D fill:#43e97b
    style E fill:#fa709a
```

---

⭐ **If you find this project helpful, please give it a star!**

**Last Updated:** December 2025
