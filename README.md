# 🚀 Launch Data Analysis Project

## 📌 Overview

This project focuses on collecting, cleaning, and analyzing launch data using Python.
The dataset is transformed from raw JSON into a structured Pandas DataFrame, followed by preprocessing steps such as handling missing values and filtering relevant records.

---

## 📊 Features

* Convert API JSON responses into a structured DataFrame
* Clean and preprocess launch data
* Handle missing values using statistical methods
* Filter specific launch conditions (e.g., remove Falcon 1 missions)
* Prepare dataset for further analysis or visualization

---

## 🛠️ Tech Stack

* Python 🐍
* Pandas
* NumPy
* Requests (for API calls)
* Jupyter Notebook

---

## ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## 🚀 Usage

Run the notebook or script:

```bash
jupyter notebook
```

or

```bash
python main.py
```

---

## 🧹 Data Processing Steps

1. Fetch data from API
2. Normalize JSON into tabular format using `pd.json_normalize()`
3. Create structured DataFrame
4. Filter unwanted records (e.g., Falcon 1 launches)
5. Handle missing values:

   * Replace `NaN` in `PayloadMass` with mean value
6. Perform exploratory data analysis

---

## 📈 Example Code

```python
# Calculate mean payload mass
mean_payload = launch_df['PayloadMass'].mean()

# Replace missing values
launch_df['PayloadMass'] = launch_df['PayloadMass'].fillna(mean_payload)
```

---

## 📁 Project Structure

```
├── data/
├── notebooks/
├── src/
├── README.md
├── requirements.txt
```

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you'd like to change.

---

## 📜 License

This project is open-source and available under the MIT License.

---

## ✨ Acknowledgements

* SpaceX API
* Pandas Documentation
* Open-source community
