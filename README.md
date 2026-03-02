# NFL Game Outcome Prediction using Machine Learning

A machine learning project to predict NFL game outcomes by reproducing and extending the work of Beal et al. (2020).

## Project Overview

This project implements and compares multiple machine learning classifiers to predict the outcomes (Win/Loss) of NFL games. The goal is to reproduce key findings from the paper "A Critical Comparison of Machine Learning Classifiers to Predict Match Outcomes in the NFL" and deploy the best-performing model on AWS SageMaker.

## Research Question

> Can machine learning algorithms accurately predict the outcomes of NFL games, and which classifier performs best for this task?

## Dataset

- **Source:** [NFL Team Stats 2002-2025 (ESPN) on Kaggle](https://www.kaggle.com/datasets/cviaxmiwnptr/nfl-team-stats-20022019-espn)
- **Size:** 6,000+ games over 20+ NFL seasons
- **Features:** 61 features per game including:
  - Points scored (home/away)
  - First downs & total yards
  - Passing & rushing statistics
  - Turnovers & penalties
  - Third/fourth down conversions
  - Time of possession

## Methodology

Following Beal et al. (2020), this project:

1. **Data Preprocessing:** Clean data, handle missing values, normalize features
2. **Feature Engineering:** Select relevant features for classification
3. **Model Training:** Implement and compare classifiers:
   - Naive Bayes
   - Random Forest
   - AdaBoost
   - Support Vector Machine (SVM)
4. **Evaluation:** Compare accuracy, precision, recall, F1-score
5. **Deployment:** Deploy best model on AWS SageMaker (stretch goal)

## Project Structure

```
NFL-Game-Prediction/
├── README.md
├── data/
│   └── (dataset files)
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_model_training.ipynb
│   └── 04_evaluation.ipynb
├── src/
│   └── (source code)
├── reports/
│   └── (final report and presentation)
└── requirements.txt
```

## Timeline

| Week | Task |
|------|------|
| Week 4-5 | Data Collection & Preprocessing |
| Week 6-7 | Model Implementation |
| Week 8-9 | AWS SageMaker Deployment |
| Week 10-11 | Evaluation & Analysis |
| Week 12 | Report Writing |
| Week 13 | Final Presentation |

## References

1. Beal, R., Norman, T. J., & Ramchurn, S. D. (2020). "A Critical Comparison of Machine Learning Classifiers to Predict Match Outcomes in the NFL." *International Journal of Computer Science in Sport*, 19(2), 36-50. https://doi.org/10.2478/ijcss-2020-0009

2. Lock, D., & Nettleton, D. (2014). "Using Random Forests to Estimate Win Probability Before Each Play of an NFL Game." *Journal of Quantitative Analysis in Sports*, 10(2), 197-205. https://doi.org/10.1515/jqas-2013-0100

3. Weirich, C., et al. (2025). "Advancing NFL Win Prediction: From Pythagorean Formulas to Machine Learning Algorithms." *Frontiers in Sports and Active Living*, 7, 1638446. https://doi.org/10.3389/fspor.2025.1638446

## Author

**Jeevith Doddalingegowda Rama**

## License

This project is for educational purposes as part of a Machine Learning course.
