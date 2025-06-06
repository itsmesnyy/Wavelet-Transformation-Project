# 📊 Feature Engineering using Signal Processing to Predict DTC and DTS Values

This project explores the use of **Wavelet Transformation** (a signal processing technique) to enhance the prediction of **DTC (Compressional Sonic Transit Time)** and **DTS (Shear Sonic Transit Time)** using machine learning models. The motivation behind this project is to improve the accuracy of subsurface property predictions by leveraging frequency-domain features extracted from well log data.

---

## 🔍 Project Objective

- Use **raw well log data** to train machine learning models for predicting DTC and DTS.
- Apply **Discrete Wavelet Transformation (DWT)** to these logs to extract compressed, denoised features.
- Re-train the model on transformed features and compare performance.
- Evaluate whether wavelet-based features offer improved accuracy.

---

## 🧠 Techniques Used

- **Signal Processing**: Discrete Wavelet Transform (`pywt`)
- **Machine Learning**: XGBoost Regressor
- **Evaluation**: RMSE, R² Score
- **Data Handling**: Pandas, NumPy
- **Visualization**: Matplotlib, Seaborn

---

## 🗂 Dataset

**Source**: Synthetic Sonic Log Curve Generation Challenge (similar to field well log data)

**Input Features**:
| Column | Description |
|--------|-------------|
| CAL    | Caliper (inches) |
| CNC    | Neutron Porosity |
| GR     | Gamma Ray (API) |
| HRD    | Deep Resistivity (Ohm·m) |
| HRM    | Medium Resistivity (Ohm·m) |
| PE     | Photo-electric Factor (Barn) |
| ZDEN   | Density (g/cc) |

**Target Variables**:
- `DTC` - Compressional Sonic Travel Time
- `DTS` - Shear Sonic Travel Time

---

## 📁 Project Structure

```bash
.
├── Wavelet Transformation project.ipynb   # Full pipeline notebook
├── train.csv                              # Training data
├── real_test_result.csv
├── test.csv                               # Test data
├── README.md                              # Project overview
