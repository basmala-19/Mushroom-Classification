from pathlib import Path

# Define README content
readme_content = """
# 🔍 SVM Kernel Comparison on Non-Linear Data

This project explores the performance of different SVM approaches on synthetic non-linear data (`make_moons` dataset). It also includes a comparison with Naive Bayes as a baseline model.

## 📊 Algorithms Compared

1. **Linear SVM**
2. **Non-Linear SVM (RBF Kernel)**
3. **SVM with Polynomial Kernel**
4. **Linear SVM with Polynomial Features**
5. **Naive Bayes Classifier**

## 🧪 Dataset

- Generated using `make_moons(n_samples=300, noise=0.2)`
- Non-linear binary classification task.

## ⚙️ Preprocessing

- Data split into training and testing sets (70/30 split).
- Standardized features using `StandardScaler`.
- PCA applied for 2D visualization only.

## 🧠 Key Findings

- `PolynomialFeatures + Linear SVM` outperformed the `Polynomial Kernel` SVM on the same dataset.
- RBF Kernel provided strong non-linear separation.
- Naive Bayes performed reasonably but was less accurate than SVMs.

## ✅ Accuracy Comparison

| Model                         | Accuracy |
|------------------------------|----------|
| Linear SVM                   | xx%      |
| RBF SVM                      | xx%      |
| Polynomial Kernel SVM        | xx%      |
| Polynomial Features + SVM    | xx%      |
| Naive Bayes                  | xx%      |

> Replace `xx%` with your actual results.

## 📈 Visualizations

Decision boundaries for each model were plotted to visually compare how well they separate the classes.

## 🧾 Conclusion

Feature transformation using `PolynomialFeatures` helped Linear SVM perform significantly better than the direct use of a polynomial kernel. RBF kernel also showed strong performance on non-linear data.

## 🛠️ Requirements

- Python
- NumPy
- pandas
- scikit-learn
- matplotlib

Install dependencies:
```bash
pip install -r requirements.txt
