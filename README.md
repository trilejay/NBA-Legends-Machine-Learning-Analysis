# Who's the GOAT? – A Machine Learning Analysis  

In this project, I apply machine learning techniques to compare the careers of Michael Jordan and LeBron James using NBA datasets from Kaggle. The goal is to explore the GOAT debate from a data-driven perspective by analyzing player performance across advanced stats and applying various ML models.  


## 🛠️ Tech Stack  
- **Python**  
- **Pandas** – data cleaning & feature engineering  
- **scikit-learn** – ML models & evaluation  
- **Matplotlib / Seaborn** – visualization
  
## Datasets  
- [Michael Jordan, Kobe Bryant, and LeBron James Stats](https://www.kaggle.com/datasets/xvivancos/michael-jordan-kobe-bryant-and-lebron-james-stats)  
- [LeBron James Regular Season Games (2003–current)](https://www.kaggle.com/datasets/zhikchen/lebron-james-regular-season-games-2003-current)  
- [Jordan vs LeBron Stats](https://www.kaggle.com/datasets/curtisguyton/jordan-vs-lebron)  

## ⚙Data Cleaning and Processing  
- Cleaned datasets by handling missing values, fixing data types, and standardizing features.  
- Engineered features such as True Shooting Percentage (TS%), Player Efficiency Rating (PER), Box Plus-Minus (BPM), and Win Shares (WS).  
- Combined multiple datasets into single tables for model training.  

## Machine Learning Models  
### Unsupervised Learning  
- **KMeans Clustering** – grouped player seasons into performance tiers.  
- **Principal Component Analysis (PCA)** – reduced dimensionality for visualization.  
- **Hierarchical Clustering** – revealed tiers of elite vs. role-player  

### Supervised Learning  
- **Linear & Logistic Regression** – modeled relationships between usage and efficiency.  
- **Decision Trees** – explained statistical differences between players.  
- **Naive Bayes (Gaussian & Multinomial)** – classified playoff stats with ~69% accuracy.  
- **Support Vector Machine (SVM)** – achieved 90%+ accuracy using RBF kernel.  

### Ensemble Methods  
- **Random Forest** – 91.2% accuracy in classifying Jordan vs. LeBron performances.  
- **AdaBoost** – 88.9% accuracy.  
- **Stacking (LR + KNN + Decision Tree → Logistic Regression)** – best performance at 91.5% accuracy.  

## 📈 Results  
- Machine learning models were able to distinguish between Jordan and LeBron with high accuracy, demonstrating clear statistical differences in their play styles.  
- Ensemble methods (Random Forest, Stacking) provided the most robust results.  
- Data-driven analysis confirmed that while both players are elite, their greatness manifests in different statistical ways.
- While models can classify games with >90% accuracy, the answer to "Who’s the GOAT?" is ultimately still subjective to the viewer. 

---

