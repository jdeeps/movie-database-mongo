# 🎬 SJSU Movie Data Analysis — MongoDB with Python

> Analysis of a movie streaming dataset using MongoDB aggregation pipelines and Python visualizations, covering customer behavior, complaints, employee metrics, and movie performance.

---

## 📌 Project Overview

This project performs data analysis on a movie streaming service database stored in **MongoDB Atlas**. Using **PyMongo** and **Python**, 17 analytical scenarios are explored through MongoDB aggregation queries, with results visualized using **Matplotlib** and **Seaborn**.

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| **MongoDB Atlas** | Cloud-hosted NoSQL database |
| **PyMongo** | Python driver for MongoDB |
| **Pandas** | Data manipulation |
| **Matplotlib / Seaborn** | Data visualization |
| **Jupyter Notebook** | Interactive analysis environment |

---

## ⚙️ Setup & Installation

### Prerequisites
- Python 3.x
- Anaconda (recommended)
- MongoDB Atlas account with the dataset loaded

### Install Dependencies

**In Anaconda environment:**
```bash
conda install mongo-tools
conda install mongodb
conda install pymongo
conda install r-mongolite
```

**Via pip:**
```bash
pip install pymongo
pip install "pymongo[srv]"
pip install pixiedust
pip install pixiedust_node
```

### MongoDB Connection

Update the connection string in the notebook with your own MongoDB Atlas credentials before running:

```python
from pymongo import MongoClient

client = MongoClient('mongodb+srv://<username>:<password>@<cluster-url>/test')
```

> ⚠️ Never hardcode credentials. Use environment variables or a config file.

---

## 📊 Analysis Scenarios

| # | Scenario | Chart Type |
|---|----------|------------|
| 1 | Number of movies watched per country | Bar chart |
| 2 | Number of movies released per year | Pie chart |
| 3 | Top 5 employees who resolved most complaints | Bar chart |
| 4 | Number of customers per country | Pie chart |
| 5 | Number of complaints per complaint category | Bar chart |
| 6 | Complaints closed per month | Bar chart |
| 7 | Complaints created per month | Pie chart |
| 8 | Payment made per month | Bar chart |
| 9 | Top 10 customers based on movies watched | Bar chart |
| 10 | Top 5 directors based on user watch history | Bar chart |
| 11 | Complaints based on severity | Pie chart |
| 12 | Average salary based on designation | Bar chart |
| 13 | Employees per designation by employment status | Table |
| 14 | 5 latest closed complaints | Table |
| 15 | Most preferred screens by customers | Pie chart |
| 16 | Top highest grossing movies | Bar chart |
| 17 | Top 5 most rated movies | Bar chart |

---

## 📁 Repository Structure

```
├── README.md                          # Project overview and setup instructions
└── Lab2_MongoWithPython_Queries.ipynb # All queries, analysis, and visualizations
```

---

## ▶️ How to Run

1. Clone the repository
2. Install all dependencies listed above
3. Set up your MongoDB Atlas cluster and load the dataset
4. Update the connection string in the notebook with your credentials
5. Open `Lab2_MongoWithPython_Queries.ipynb` in Jupyter
6. Run all cells in order

---

## 🗄️ Database Details

- **Database:** `data225_lab2`
- **Collection:** `smd`
- **Platform:** MongoDB Atlas (Cloud)
