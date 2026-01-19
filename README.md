
# Correlation Between Light Conditions and Road Accidents

**Coursera Capstone Project**
**Author:** Lyba Mughees
**Date:** August 29, 2020

---

## 📌 Project Overview

Road accidents are a major global concern, impacting millions of people every year. While many accidents are not life-threatening, their increasing frequency places a significant burden on society due to rising medical and recovery costs.

According to global statistics:

* Approximately **1.35 million people die** in road crashes annually
* Around **50 million people suffer serious but non-life-threatening injuries**
* Governments spend an estimated **$10.7 billion** on medical costs related to road accidents

This project investigates whether **lighting conditions** play a role in the occurrence and severity of road accidents. Specifically, it explores whether accidents are more frequent in poorly lit areas, under the assumption that lighting may be an easier factor to improve through infrastructure changes.

---

## 🎯 Objective

The primary goal of this analysis is to examine the correlation between:

* **Light Conditions (`LIGHTCOND`)**
* **Accident Severity (`SEVERITYCODE`)**
* **Address Type (e.g., alley vs. intersection)**

The intent is to determine whether darker environments contribute to a higher number or severity of road accidents.

---

## 🧪 Methodology

### Tools & Technologies

* **IBM Watson Studio** – Data analysis notebook
* **GitHub** – Version control and project repository
* **Python Libraries Used:**

  * Pandas
  * NumPy
  * Seaborn
  * Matplotlib

### Data Processing Steps

1. Uploaded the CSV dataset directly into Watson Studio.
2. Inspected data types using `df.dtypes`.

   * `SEVERITYCODE`: `int64`
   * `LIGHTCOND`: `object`
   * `ADDRTYPE`: `object`
3. Focused analysis on severity, lighting conditions, and address types.
4. Used value counts to identify where most accidents occur, comparing darker areas (alleys) with well-lit locations (intersections).
5. Created a filtered DataFrame containing only relevant columns to simplify analysis.

---

## 📊 Results

* An initial attempt to analyze correlations using `sns.regplot` resulted in data type errors.
* Converting `LIGHTCOND` to a numeric type (float) also resulted in errors.
* These issues suggest that:

  * The selected variables may not have a strong linear relationship
  * Lighting conditions may not significantly influence accident location or frequency

---

## 💬 Discussion

The lack of meaningful correlation indicates that **lighting conditions alone may not be a strong predictor of road accidents**. Other variables—such as speed, driver behavior, or road design—may play a more significant role.

Future analyses could explore:

* Speed vs. severity
* Weather conditions vs. accident frequency
* Time of day vs. severity

---

## ✅ Conclusion

The results of this analysis did not align with the initial hypothesis. The data suggests that **lighting conditions do not have a strong impact on the number or severity of road accidents**. While improving lighting may still enhance road safety in other ways, it does not appear to be a primary contributing factor based on this dataset.

Choosing a different set of variables may yield stronger correlations and more actionable insights in future studies.

---

## 📂 Repository Contents

* `Data for Capstone.ipynb` – Data analysis and visualizations
* `README.md` – Project documentation

---

## 📬 Contact

If you have questions or suggestions, feel free to reach out or open an issue in this repository.
