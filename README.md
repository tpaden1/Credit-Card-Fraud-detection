# Credit-Card-Fraud-detection

**Trevor Paden | December 6, 2025**

A machine learning project comparing Logistic Regression and Random Forest for detecting credit card fraud on a highly imbalanced dataset.

---

## About This Project

I built this for my machine learning final project. The goal was to detect fraudulent credit card transactions when fraud makes up only 0.17% of all transactions - a tough problem because of the extreme imbalance.

I tested two approaches:
- **Logistic Regression** - simple and fast
- **Random Forest** - more complex, better results

**Bottom line:** Random Forest works way better for real-world use. It catches 85% of fraud with only 115 false alarms, compared to Logistic Regression's 1,458 false alarms.

---

## The Data

**Dataset:** [Kaggle Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?resource=download)

- 284,807 transactions
- Only 492 are fraud (0.17%!)
- 30 features (mostly PCA-transformed for privacy)

**Note:** I couldn't include the dataset in this repo because it's ~150MB. You'll need to download it from Kaggle yourself and save it as `creditcard.csv` in the same folder as the notebook.

---

## How to Run This

1. **Download the data** from the link above
2. **Install packages:**
```bash
   pip install pandas numpy scikit-learn imbalanced-learn matplotlib seaborn jupyter
```
3. **Run the notebook:**
```bash
   jupyter notebook Credit_Fraud_Final.ipynb
```
4. **Run all cells** (Kernel → Restart & Run All)

That's it. Should take about 5 minutes to run everything.
(takes me around 2-3 minutes)

---

## Results

| Model | Precision | Recall | False Positives |
|-------|-----------|--------|-----------------|
| Logistic Regression | 6% | 92% | 1,458  |
| Random Forest | 42% | 85% | 115  |

Random Forest is the clear winner it catches most fraud without overwhelming you with false alarms.

---

## What I Learned

- Class imbalance is a real pain; you can't just use accuracy
- SMOTE really helps models learn from imbalanced data
- Sometimes the simpler model (Logistic Regression) isn't the best choice
- Trade-offs matter; catching 7 more frauds isn't worth 1,343 more false alarms

---

## Tools Used

- Python, Jupyter Notebook
- Scikit-learn, Pandas, NumPy
- Matplotlib, Seaborn
- Imbalanced-learn (for SMOTE)

---

## Acknowledgments

**Dataset:** ULB Machine Learning Group via Kaggle

**AI Help:** I used ChatGPT and Claude AI to help structure my written report and proofread for grammar/clarity. All the code, analysis, and actual work is mine - the AI just helped me write it up better.

---

## Contact

Questions? Feel free to reach out!

**Trevor Paden**  
tpaden1@charlotte.edu
