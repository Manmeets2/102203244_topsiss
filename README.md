Here's your complete, enhanced, and **single `README.md`** file ready to be copied into your GitHub repository. It includes all code, structure, features, usage, and author info in a clean and stylish way.

---

### ✅ Final `README.md` content:

```markdown
# 🧠 TOPSIS Decision Support Tool

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen.svg)]()
[![Author](https://img.shields.io/badge/Author-Manmeet%20Singh-orange.svg)]()

> A Python package implementing **TOPSIS** — an MCDM (Multi-Criteria Decision-Making) method to rank alternatives based on multiple attributes.

---

## 📌 What is TOPSIS?

**TOPSIS** (Technique for Order of Preference by Similarity to Ideal Solution) is a well-established decision-making method that:
- Identifies the **positive ideal solution** (most desirable)
- Identifies the **negative ideal solution** (least desirable)
- Ranks alternatives based on their **closeness to the ideal solution**

It's useful in scenarios like product comparison, supplier selection, performance analysis, etc.

---

## 📁 Project Structure

```

102203244\_topsiss/
├── topsis/
│   └── topsis.py          # Core algorithm
├── 102203244.py           # Command-line script
├── input.csv              # Sample input data
├── output.csv             # Result after TOPSIS
├── requirements.txt       # Dependencies
└── README.md              # This file

````

---

## 🚀 Features

- Simple CLI usage
- Clean output with scores and rankings
- Supports weighted and impacted criteria
- Lightweight and dependency-free (except `pandas` and `numpy`)

---

## 🔧 Installation

### ✅ Option 1: Clone and install requirements

```bash
git clone https://github.com/Manmeets2/102203244_topsiss.git
cd 102203244_topsiss
pip install -r requirements.txt
````

### ✅ Option 2: Install as a package (for local development)

```bash
pip install .
```

---

## 🧪 Sample Input Format (`input.csv`)

The input should have the following format:

| Model   | Feature1 | Feature2 | Feature3 | Feature4 |
| ------- | -------- | -------- | -------- | -------- |
| Model A | 250      | 16       | 12       | 5        |
| Model B | 200      | 16       | 8        | 3        |

* The **first column** is treated as the name/identifier (excluded from calculations).
* All other columns are treated as numerical attributes.

---

## 🛠️ Usage

### ▶️ Run from command line:

```bash
python 102203244.py <input_file.csv> <weights> <impacts> <output_file.csv>
```

### 📥 Arguments:

* `input_file.csv`: Path to input CSV file
* `weights`: Comma-separated values, e.g., `1,1,1,1`
* `impacts`: Comma-separated `+` (beneficial) or `-` (non-beneficial), e.g., `+,+,-,+`
* `output_file.csv`: Output file path

---

### ✅ Example

```bash
python 102203244.py input.csv 1,1,1,1 +,+,-,+ output.csv
```

---

## 📤 Output (`output.csv`)

The output will be a CSV like:

| Model   | Feature1 | Feature2 | Feature3 | Feature4 | Topsis Score | Rank |
| ------- | -------- | -------- | -------- | -------- | ------------ | ---- |
| Model A | 250      | 16       | 12       | 5        | 0.6785       | 1    |
| Model B | 200      | 16       | 8        | 3        | 0.4321       | 2    |

---

## 🧠 How TOPSIS Works

1. **Normalize** the input decision matrix
2. **Apply weights** to each column
3. Identify the **ideal best** and **ideal worst**
4. Compute the **Euclidean distance** to both
5. Calculate **relative closeness (Topsis Score)**
6. Assign **rank** based on the score

---

## 🧑‍🎓 Author

* **Name:** Manmeet Singh
* **Roll Number:** 102203244
* **Institute:** IIT Ropar
* **Assignment:** Python Programming (TOPSIS Implementation)

---

## 📃 License

This project is licensed under the [MIT License](LICENSE).

---

## ⭐️ Star This Repo

If you found this useful, consider giving a ⭐ to help others discover this work.

> Made with ❤️ to simplify decision-making using Python.

````

---

✅ **To add this to your project:**
1. Copy the entire markdown content above.
2. Paste it into your `README.md` file inside your GitHub repo.
3. Save, commit, and push:
   ```bash
   git add README.md
   git commit -m "Add enhanced README"
   git push
````
