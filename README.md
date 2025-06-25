# 📊 CGPA Analysis Dashboard

## Student Academic Performance Analysis & Visualization

A comprehensive Python-based data analysis project for analyzing and visualizing CGPA (Cumulative Grade Point Average) data of shortlisted students from IIIT Bhubaneswar.

---

## 🎯 **Project Overview**

This project provides deep insights into academic performance patterns, helping educational institutions make data-driven decisions for student support, resource allocation, and academic planning. The analysis covers 152 shortlisted students across different engineering branches.

### **Key Features**
- 📈 Comprehensive statistical analysis of CGPA data
- 🎨 Interactive visualizations and dashboards
- 🏫 Branch-wise performance comparison
- 📊 Performance level categorization
- 🔍 Top and bottom performer identification
- 📋 Actionable recommendations for academic improvement

---

## 🛠️ **Technologies Used**

| Technology | Purpose |
|------------|---------|
| **Python 3.8+** | Core programming language |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical computations |
| **Matplotlib** | Static visualizations |
| **Seaborn** | Statistical visualizations |
| **SciPy** | Statistical tests and analysis |

---


## 🚀 **Getting Started**

### **Prerequisites**
- Python 3.8 or higher
- pip package manager

### **Installation**


### **Quick Start**

```python
# Run the main analysis
python src/cgpa_analysis.py

# Generate visualizations
python src/visualizations.py
```

---

## 📊 **Analysis Features**

### **1. Basic Statistics**
- Mean, Median, Mode analysis
- Standard deviation and variance
- Quartile analysis (Q1, Q2, Q3)
- Range and interquartile range (IQR)

### **2. Distribution Analysis**
- CGPA category distribution
- Performance level classification
- Normality testing (Shapiro-Wilk test)
- Skewness and kurtosis analysis

### **3. Branch-wise Comparison**
- Department-wise performance metrics
- Statistical significance testing (ANOVA)
- Performance level distribution by branch
- Comparative analysis across departments

### **4. Performance Insights**
- Top 10 performers identification
- Students needing academic support
- Percentile rankings (10th, 25th, 50th, 75th, 90th, 95th, 99th)
- Risk assessment categories

---

## 📈 **Visualizations**

The project generates six comprehensive visualizations:

| Visualization | Description | Insights |
|---------------|-------------|----------|
| **CGPA Distribution** | Histogram with mean/median lines | Overall performance spread |
| **Branch-wise Box Plot** | Performance comparison by department | Departmental variations |
| **Performance Pie Chart** | Distribution of performance levels | Achievement categories |
| **Rank vs CGPA Plot** | Performance gradient visualization | Individual positioning |
| **Bar Chart** | Average CGPA by branch | Branch comparison |
| **Cumulative Distribution** | Percentile analysis | Performance benchmarking |

---

## 🎯 **Key Insights**

### **Performance Metrics**
- **Overall Mean CGPA**: 7.74/10.0
- **Performance Distribution**: 45% Excellent, 35% Very Good, 18% Good, 2% Needs Improvement
- **Top Performer**: CGPA 9.44
- **Academic Risk**: Students with CGPA < 7.0

### **Statistical Findings**
- **Distribution**: Slightly left-skewed (more high performers)
- **Consistency**: Moderate variability (σ = 0.88)
- **Branch Differences**: Statistically significant variations across departments

---

## 📋 **Usage Examples**

### **Basic Analysis**
```python
import pandas as pd
from src.cgpa_analysis import CGPAAnalyzer

# Load data
analyzer = CGPAAnalyzer('data/student_data.csv')

# Get basic statistics
stats = analyzer.get_basic_stats()
print(stats)

# Generate performance report
report = analyzer.generate_report()
```

### **Custom Visualizations**
```python
from src.visualizations import create_dashboard

# Create custom dashboard
create_dashboard(
    data=df,
    save_path='output/plots/',
    title='Custom CGPA Analysis'
)
```

---

## 📊 **Sample Output**

```
==========================================
COMPREHENSIVE CGPA ANALYSIS
==========================================

BASIC STATISTICS
----------------------------------------
Total Students: 152
Mean CGPA: 7.743
Median CGPA: 7.690
Standard Deviation: 0.876
Range: 4.020

PERFORMANCE DISTRIBUTION
----------------------------------------
Excellent (8.0-10.0): 68 students (44.7%)
Very Good (7.0-8.0): 53 students (34.9%)
Good (6.0-7.0): 28 students (18.4%)
Needs Improvement (<6.0): 3 students (2.0%)
```

---

## 🔬 **Advanced Features**

### **Statistical Tests**
- **Normality Testing**: Shapiro-Wilk test for distribution analysis
- **ANOVA**: One-way analysis of variance for branch comparison
- **Correlation Analysis**: Relationship between different performance metrics

### **Performance Categorization**
- **Risk Assessment**: Automatic identification of at-risk students
- **Excellence Recognition**: Top performer identification
- **Peer Group Analysis**: Similar performance group formation

---

## 🎯 **Recommendations Generated**

The analysis automatically generates actionable recommendations:

- **Academic Support**: Targeted intervention for low performers
- **Peer Mentoring**: Pairing high and low performers
- **Resource Allocation**: Branch-wise support distribution
- **Recognition Programs**: Top performer acknowledgment
- **Early Warning Systems**: Proactive student monitoring

---

## 📄 **License**

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 **Acknowledgments**

- **IIIT Bhagalpur** for providing the dataset
- **Python Community** for excellent data science libraries

---

## 📚 **Future Enhancements**

- [ ] Interactive web dashboard using Plotly/Dash
- [ ] Machine learning predictions for academic performance
- [ ] Integration with institutional databases
- [ ] Real-time performance monitoring
- [ ] Mobile app for student performance tracking
- [ ] Advanced analytics with predictive modeling

---

**Made with ❤️ for educational data analysis**

---

*Last updated: June 2025*
