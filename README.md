 DL_Project_Weather_Prediction_System
# 🌦️ Weather Prediction System — Deep Learning Model

Developed a Deep Learning model for weather prediction using a Sequential Neural Network with inputs — precipitation, temp_max, temp_min, and wind. Optimized using Adam and trained with cross-entropy loss, the model achieved 82% accuracy. It classifies weather conditions into rain, drizzle, fog, sun, or snow, using argmax for final class label prediction.
## 📘 Project Description

The **Weather Prediction System** is a Deep Learning-based project that predicts the type of weather (Rain, Drizzle, Fog, Sun, or Snow) using meteorological features such as **precipitation, temperature, and wind speed**.
Built with a **Sequential Neural Network**, this model achieves around **82% accuracy**, making it a robust baseline for short-term weather classification tasks.

---

## 🔍 About the Project

This project demonstrates how deep learning can be applied to real-world meteorological data to predict weather conditions.
It uses historical Seattle weather data and applies data preprocessing, normalization, model training, and evaluation to classify weather types accurately.

---

## 🧠 Model Architecture

The model is a **Sequential Neural Network** built using **TensorFlow/Keras**, consisting of:

* **Input Layer:** Features — `precipitation`, `temp_max`, `temp_min`, and `wind`
* **Hidden Layers:** Fully connected `Dense` layers using **ReLU** activation
* **Output Layer:** Uses **Softmax** activation for multi-class classification
* **Optimizer:** **Adam**
* **Loss Function:** **Categorical Cross-Entropy**
* **Metric:** **Accuracy**

The model uses **argmax** on the final predictions to determine the most probable weather class.

---

## 🧾 Dataset Description

The dataset used is **Seattle Weather Data (2012–2015)** containing **1,461 daily records**.

| Column          | Description                                                   |
| :-------------- | :------------------------------------------------------------ |
| `date`          | Date of observation                                           |
| `precipitation` | Daily precipitation (mm)                                      |
| `temp_max`      | Maximum temperature (°C)                                      |
| `temp_min`      | Minimum temperature (°C)                                      |
| `wind`          | Wind speed (m/s)                                              |
| `weather`       | Categorical weather condition (rain, drizzle, fog, sun, snow) |

The target variable **`weather`** is label-encoded before training.

---

## ⚙️ Tech Stack & Libraries

**Languages:**

* Python 🐍

**Libraries & Frameworks:**

* **TensorFlow / Keras** – Deep Learning Model
* **NumPy** – Numerical Computations
* **Pandas** – Data Handling
* **Matplotlib** – Visualization
* **Scikit-learn (sklearn)** – Preprocessing, Label Encoding, and Data Splitting

---

## 🚀 Features

* Predicts weather types using deep learning
* Handles real meteorological data
* Trained using Adam optimizer and cross-entropy loss
* Achieves ~82% accuracy on test data
* Easy to retrain with updated weather datasets

---

## 📊 Results

The trained model achieved **~82% accuracy**, effectively classifying weather types like Rain, Drizzle, Fog, Sun, and Snow.

---

## 📁 Repository Structure

```
📦 DL_Project_Weather_Prediction_System
│
├── ibm_dl_model_weather_prediction.ipynb   # Jupyter Notebook with full project code
├── seattle-weather.csv                     # Dataset used for training
└── README.md                               # Project documentation (this file)
```

---

## 🧪 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/DL_Project_Weather_Prediction_System.git
   cd DL_Project_Weather_Prediction_System
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Run the notebook:

   ```bash
   jupyter notebook ibm_dl_model_weather_prediction.ipynb
   ```

4. Train and test the model — predictions will be shown at the end.

---

## 📈 Future Improvements

* Integrate live weather data APIs
* Use LSTM or CNN for sequence-based time-series forecasting
* Deploy model using Flask or Streamlit for real-time predictions
