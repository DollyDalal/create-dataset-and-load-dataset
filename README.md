# 📊 Data Creation and Loading Guide

![Data Banner](https://via.placeholder.com/1000x300.png?text=Data+Creation+and+Loading+Project)

## 🚀 Overview

This project demonstrates how to:

✅ Create a sample dataset  
✅ Save the dataset to a CSV file  
✅ Load the dataset for analysis  

We use **Python 🐍** with the **pandas** library.

---

## 🛠️ Requirements

Make sure you have the following installed:

- Python 3.x
- pandas
- numpy (optional but recommended)

Install dependencies using:

```bash
pip install pandas numpy
```

---

## 📁 Project Structure

```
project-folder/
│
├── create_data.py
├── load_data.py
├── sample_data.csv
└── README.md
```

---

# 🧱 Step 1: Create Sample Data

The following script creates a dataset and saves it as a CSV file.

```python
import pandas as pd
import numpy as np

# Create sample data
data = {
    "ID": range(1, 11),
    "Name": ["Alice", "Bob", "Charlie", "David", "Eva",
             "Frank", "Grace", "Helen", "Ian", "Jane"],
    "Age": np.random.randint(18, 60, size=10),
    "Salary": np.random.randint(30000, 100000, size=10)
}

# Convert dictionary to DataFrame
df = pd.DataFrame(data)

# Save to CSV file
df.to_csv("sample_data.csv", index=False)

print("✅ Sample data created and saved as sample_data.csv")
```

### 📸 Example Output File

![CSV Example](https://via.placeholder.com/800x400.png?text=Sample+CSV+File+Preview)

---

# 📥 Step 2: Load the Dataset

Use the following script to load and view the dataset.

```python
import pandas as pd

# Load dataset
df = pd.read_csv("sample_data.csv")

# Display first 5 rows
print(df.head())
```

---

## 🖥️ Running the Project

### ▶️ Run Data Creation Script

```bash
python create_data.py
```

### ▶️ Run Data Loading Script

```bash
python load_data.py
```

---

## 📊 Example Console Output

```
   ID     Name  Age  Salary
0   1    Alice   25   54000
1   2      Bob   42   72000
2   3  Charlie   31   61000
```

---

## 💡 Customization Ideas

✨ Add more columns (Email, Department, City)  
✨ Generate larger datasets  
✨ Export to Excel instead of CSV  
✨ Connect to a database  

---

## 📈 Data Workflow Diagram

![Workflow Diagram](https://via.placeholder.com/900x400.png?text=Create+Data+→+Save+CSV+→+Load+Data+→+Analyze)

---

## 📜 License

This project is open-source and free to use 🎉

---

## 🙌 Author

Created for learning and demonstration purposes.

Happy Coding! 🚀🐍
