# Who's the GOAT? – A Machine Learning Analysis  

- In this project, I apply machine learning techniques to compare the careers of Michael Jordan and LeBron James using NBA datasets from Kaggle. The goal is to explore the GOAT debate from a data-driven perspective by analyzing player performance across advanced stats and applying various ML models. 
- The repo contains a PDF document summarizing and outlining the steps I took for analysis. It includes detailed planning of the project, actionable steps I took towards analysis, code-snippets of preparing the data and training the models, as well as screenshots of visual analyses.

## Tech Stack  
- **Python**  
- **Pandas** – data cleaning & feature engineering  
- **scikit-learn** – ML models & evaluation  
- **Matplotlib / Seaborn** – visualization
  
## Datasets  
- [Michael Jordan, Kobe Bryant, and LeBron James Stats](https://www.kaggle.com/datasets/xvivancos/michael-jordan-kobe-bryant-and-lebron-james-stats)  
- [LeBron James Regular Season Games (2003–current)](https://www.kaggle.com/datasets/zhikchen/lebron-james-regular-season-games-2003-current)  
- [Jordan vs LeBron Stats](https://www.kaggle.com/datasets/curtisguyton/jordan-vs-lebron)  

## Data Cleaning and Processing  
- Cleaned datasets by handling missing values, fixing data types, and standardizing features.  
- Engineered features such as True Shooting Percentage (TS%), Player Efficiency Rating (PER), Box Plus-Minus (BPM), and Win Shares (WS).  
- Combined multiple datasets into single tables for model training.  

## Machine Learning Models  
### Unsupervised Learning  
- **Clustering** – Used K-Means Clustering and PCA to group similar player-seasons together without any pre-defined labelsgrouped player seasons into performance tiers (role palyer, below-avg player, or star player). Jordan and Lebron were consistently clustered together under "Star Player" tier. This model proves that greatness actually does have a statistical signature that ML models can detect objectively.
<img width="889" height="281" alt="image" src="https://github.com/user-attachments/assets/848963e9-2858-4e6c-a080-3527d6a83b5a" />
<img width="858" height="856" alt="image" src="https://github.com/user-attachments/assets/566027b7-3dfd-4dd2-8181-1e134ec356d3" />

- **Principal Component Analysis (PCA)** – reduced dimensionality for visualization.  
- **Hierarchical Clustering** – revealed tiers of elite vs. role-player  

### Supervised Learning  
- **Linear & Logistic Regression** – modeled relationships between usage and efficiency.
<img width="864" height="559" alt="image" src="https://github.com/user-attachments/assets/0f5b30f4-82b1-46fd-81c0-2c6cf0e88c2d" />
<img width="926" height="557" alt="image" src="https://github.com/user-attachments/assets/4d2792c5-0ece-4768-8e40-998ea980e33f" />

- **Decision Trees** – explained statistical differences between players.  
- **Naive Bayes (Gaussian & Multinomial)** – classified playoff stats with ~69% accuracy.  
- **Support Vector Machine (SVM)** – This was the star classifier. The RBF kernel achieved over 90% accuracy. This is a key result because it means Jordan and LeBron have statistically distinct features in their box score data. The model can look at a line of stats and say with high confidence, "This is a LeBron game," or "This is a Jordan game."

### Ensemble Methods  
- **Random Forest** – 91.2% accuracy in classifying Jordan vs. LeBron performances.  
- **AdaBoost** – 88.9% accuracy.  
- **Stacking (LR + KNN + Decision Tree → Logistic Regression)** – best performance at 91.5% accuracy.  

## Results  
- This project didn't declare a single winner... but it provided a data-backed framework for the debate.
- The key insight here is that Jordan and LeBron are statistically distinct. The incredibly high accuracy of my classifiers proves that their styles of greatness are different but both are uniquely identifiable by machine learning models. Especially seen in the Support Vector Machine - the model was able to classify Jordan games from Lebron games with high accuracy. Combine this with the results of the clustering analysis, which verified that both Lebron and Jordan were consistently clustered into "Star Player" category, and we can come to the following conclusion:
- There is no single answer. It depends on what you value: Jordan's peak scoring dominance and legendary status, OR LeBron's  all around versatility and longevity. These ML models can identify which style is which, but they can't decide which one is "better". That's where the debate lives on, and that's where statistics can't help.




---

