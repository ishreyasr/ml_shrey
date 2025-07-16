# Shreyas

**Transforming complex ML algorithms into simple, one-line imports**

A collection of algorithms by Shreyas, packaged as a Python library

**Portfolio:** [https://shreyuse.vercel.app/](https://shreyuse.vercel.app/)

---

## Installation

Install Library: [ml-shrey on PyPI](https://pypi.org/project/ml-shrey/)
```bash
pip install ml-shrey
```

**Best practice:** To ensure you are using the correct Python interpreter, use:
```bash
python -m pip install ml-shrey
```
## Global Installation

To install the package globally (for all users or system-wide), use:
```bash
python -m pip install --user ml-shrey
```
Or, for a true system-wide install (may require admin rights):
```bash
python -m pip install ml-shrey
```

**Note:**
- Global installs affect all Python projects on your system. For most use cases, a virtual environment is recommended to avoid version conflicts.
- On Linux/macOS, you may need to use `sudo` for a system-wide install:
  ```bash
  sudo python3 -m pip install ml-shrey
  ```
- On Windows, make sure your PATH includes the Scripts directory of your Python installation.

### After Installation: Verify & Setup

#### 1. Verify Installation
After installing, check that the package is installed and see its details:
```bash
pip show ml-shrey
```
This will display the version, summary, and the installation path (Location). You can use this path to confirm which Python environment has the package.

#### 2. Select the Correct Python Interpreter
- **VS Code:**
  1. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on Mac)
  2. Type "Python: Select Interpreter" and select it
  3. Choose the interpreter that matches the path shown in `pip show ml-shrey`
- **IDLE:**
  - Open IDLE from the same Python installation where you installed the package (check the path in `pip show ml-shrey`)
- **PyCharm:**
  1. Go to `File > Settings > Project > Python Interpreter`
  2. Select the interpreter matching the path from `pip show ml-shrey`
  3. If needed, add a new interpreter and point it to the correct Python executable

#### 3. Troubleshooting
- If you get `ModuleNotFoundError`, double-check that your script is using the same Python interpreter where `ml-shrey` is installed.
- Use `pip list` to see all installed packages in the current environment.
- To reinstall: `pip uninstall ml-shrey && pip install ml-shrey`

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
import ml_shrey as ml
ml.candidate("your_data.csv")
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
import ml_shrey as ml
ml.id3("your_data.csv")
```

---

### 3. Backpropagation (Neural Net XOR)
Runs on the XOR dataset (no CSV required).
```python
import ml_shrey as ml
ml.backpropagation(iterations=1000)
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
import ml_shrey as ml
ml.naive_bayes("your_data.csv")
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
import ml_shrey as ml
ml.kmeans("your_data.csv")
```

---

### 6. k-Nearest Neighbor (KNN)
Runs on the Iris dataset (no CSV required).
```python
import ml_shrey as ml
ml.knn()
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
import ml_shrey as ml
ml.lwlr("your_data.csv")
```

---

### 8. Support Vector Machine (SVM)
Runs on synthetic data (no CSV required).
```python
import ml_shrey as ml
ml.svm()
```

---

### 9. Random Forest
Runs on the breast cancer dataset (no CSV required).
```python
import ml_shrey as ml
ml.randomforest()
```

---

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.

## Contact

For questions, collaborations, or feedback, contact: [ishreyasr@gmail.com](mailto:ishreyasr@gmail.com)

## Attribution

Developed and maintained by Shreyas. If you use this library, please provide appropriate attribution and a link to the project or my portfolio.

