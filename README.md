# ✈️ Booking Success Rate Analysis

> **Data analysis of booking success and failure patterns using Python and Pandas.**

---

## 📊 Project Overview

This project analyzes booking data to identify the main factors associated with **successful and unsuccessful bookings**.

The analysis includes:

* 📅 Advance Purchase (AP)
* 🏢 Success rate by provider
* 📱 Success rate by device and purchase hour
* ⚠️ Failure patterns by step and error
* 🌐 Website impact
* 📏 Distance impact
* 🧳 Baggage impact
* 💺 Seat selection analysis

---

## 🔍 Main Finding

The analysis identifies a **strong decrease in booking success rate for Tablet users between 15:00 and 18:00**.

The strongest associated failure pattern is:

| Variable  | Finding       |
| --------- | ------------- |
| 📱 Device | `Tablet`      |
| 🕐 Time   | `15:00–18:00` |
| 🔄 Step   | `KO_ONLINE`   |
| ⚠️ Error  | `F`           |

The combination of `KO_ONLINE` and `F` represents the dominant failure pattern during the problematic period.

Other variables, such as **website** and **distance**, show similar decreases across their categories and therefore do not appear to be the primary cause.

---

## 📓 Notebook

The complete analysis, including data preparation, calculations, visualizations and conclusions, is available in:

👉 **[`analysis.ipynb`](analysis.ipynb)**

The notebook can be opened directly in GitHub or executed using Jupyter Notebook / VS Code.

---

## 🗂️ Dataset

The analysis uses the `Python.csv` dataset containing booking information such as:

* Purchase date and hour
* Website
* Device
* Departure date
* Providers
* Distance
* Booking status
* Booking step
* Error
* Seat
* Baggage

---

## 🛠️ Technologies

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-blue?logo=pandas)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)

The project uses:

* **Python**
* **Pandas**
* **Matplotlib**
* **Jupyter Notebook**

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone YOUR_REPOSITORY_URL
cd booking-analysis
```

### 2. Install the dependencies

```bash
pip install -r requirements.txt
```

### 3. Open the notebook

```bash
jupyter notebook analysis.ipynb
```

Alternatively, open `analysis.ipynb` directly in **VS Code**.


---

## 📝 Conclusion

The analysis suggests that the main issue is associated with a **time-specific technical problem affecting Tablet users during the online booking process**, particularly between **15:00 and 18:00**.

The `KO_ONLINE` / `F` failure pattern is the strongest indicator observed in the data.

However, the analysis does not establish causality, and additional investigation would be required to confirm the technical root cause.
