# Shreyas

A collection of 9 lab programs by Shreyas, packaged as a Python library.

**Portfolio:** [https://shreyuse.vercel.app/](https://shreyuse.vercel.app/)

## Installation

Install Library: [ml-shrey on PyPI](https://pypi.org/project/ml-shrey/)
```bash
pip install ml-shrey
```

## Usage

After installation, you can use the lab programs from anywhere:

---

### 1. Candidate Elimination
**Download the sample CSV file here:** [Download candidate.csv](https://drive.google.com/file/d/17pcKltrDMxarDD-aRLfdV-i6QqW8TM9T/view?usp=sharing)

Example CSV:
```
Sky,Temp,Humidity,Wind,Water,Forecast,EnjoySport
Sunny,Warm,Normal,Strong,Warm,Same,Yes
Rainy,Cold,High,Strong,Warm,Change,No
...
```
Usage:
```python
from ml_shrey.candidate import candidate_elimination
candidate_elimination("your_data.csv")
```

---

### 2. ID3 Decision Tree
**Download the sample CSV file here:** [Download id3.csv](https://drive.google.com/file/d/1DrMaDPUcOMPjtqy7QeSBlCmuOYlHMVl0/view?usp=sharing)

Example CSV:
```
Outlook,Temperature,Humidity,Wind,PlayTennis
Sunny,Hot,High,Weak,No
Overcast,Hot,High,Strong,Yes
...
```
Usage:
```python
from ml_shrey.id3_algo import decision_tree_from_csv
decision_tree_from_csv("your_data.csv")
```

---

### 3. Backpropagation (Neural Net XOR)
Runs on the XOR dataset (no CSV required).
```python
from ml_shrey.backpropogation import train_xor
train_xor(iterations=1000)
```

---

### 4. Naive Bayes
**Download the sample CSV file here:** [Download navie_bayes.csv](https://drive.google.com/file/d/1iUWVu_Pn2DfqQJ0mO9VwsI6JTILp6Qpi/view?usp=sharing)

Example CSV:
```
5.1,3.5,1.4,0.2,0
4.9,3.0,1.4,0.2,0
...
```
Usage:
```python
from ml_shrey.navie_bayes import run_naive_bayes
run_naive_bayes("your_data.csv")
```

---

### 5. EM & KMeans Clustering
**Download the sample CSV file here:** [Download kmeans.csv](https://drive.google.com/file/d/17i1HeUzUGQGoIwSA9yvHu7L6rNWTsyfV/view?usp=sharing)

Example CSV:
```
V1,V2
1.2,3.4
2.3,4.5
...
```
Usage:
```python
from ml_shrey.kmeans import run_clustering
run_clustering("your_data.csv", k=3, gmm_components=3)
```

---

### 6. k-Nearest Neighbor (KNN)
Runs on the Iris dataset (no CSV required).
```python
from ml_shrey.knn import run_knn_iris
run_knn_iris(test_size=0.4, random_state=1, neighbors=1)
```

---

### 7. Locally Weighted Linear Regression (LWLR)
**Download the sample CSV file here:** [Download lwlr.csv](https://drive.google.com/file/d/12lhuA1inDnukW0bBfLC31ZYAA1mNgd4-/view?usp=sharing)

Example CSV:
```
total_bill,tip
34.5,5.0
23.1,3.2
...
```
Usage:
```python
from ml_shrey.lwlr import run_lwlr
run_lwlr("your_data.csv", tau=0.5)
```

---

### 8. Support Vector Machine (SVM)
Runs on synthetic data (no CSV required).
```python
from ml_shrey.svm import run_svm_demo
run_svm_demo()
```

---

### 9. Random Forest
Runs on the breast cancer dataset (no CSV required).
```python
from ml_shrey.randomforest import RandomForest
from sklearn import datasets
from sklearn.model_selection import train_test_split
from sklearn.metrics import accuracy_score, confusion_matrix

# Load dataset
X, y = datasets.load_breast_cancer(return_X_y=True)

# Split dataset
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state=1)

# Train Random Forest
model = RandomForest(n_trees=10, max_depth=10)
model.fit(X_train, y_train)

# Predict and evaluate
y_pred = model.predict(X_test)

print("Accuracy:", accuracy_score(y_test, y_pred))
print("Confusion Matrix:\n", confusion_matrix(y_test, y_pred))
```

---

## License

This project is licensed under the MIT License. See the [LICENSE](../LICENSE) file for details.

## Contact

For questions, collaborations, or feedback, contact: [ishreyasr@gmail.com](mailto:ishreyasr@gmail.com)

## Attribution

Developed and maintained by Shreyas. If you use this library, please provide appropriate attribution and a link to the project or my portfolio. 