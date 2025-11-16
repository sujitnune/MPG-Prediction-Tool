# 🚗 MPG Prediction Tool

This project predicts vehicle fuel efficiency (MPG) using a machine learning model. It consists of two main parts:
1.  **`ML_Proj.ipynb`**: A Python Jupyter Notebook that details the data analysis, preprocessing, model training, and evaluation for predicting MPG.
2.  **`index.html`**: A client-side web application that provides an interactive user interface for getting real-time MPG estimates based on the model's findings.

---

## 🚀 Demo

The `index.html` file is a live, interactive demo. You can open it in any web browser to use the tool.


---

## ✨ Features

### Machine Learning Model (`ML_Proj.ipynb`)
* **Data Analysis (EDA):** Includes histograms, boxplots, and a correlation heatmap to understand the "Auto MPG" dataset.
* **Data Preprocessing:** Implements **One-Hot Encoding** for the categorical 'Origin' feature and **StandardScaler** for all numerical features.
* **Model Comparison:** Trains and evaluates 7 different regression models:
    * Linear, Ridge, and Lasso Regression
    * Decision Tree Regressor
    * Support Vector Regressor (SVR)
    * Gradient Boosting Regressor
    * **Random Forest Regressor** (Best performance)
* **Model Evaluation:** The final Random Forest model achieves an **R² score of 0.933**.

### Web Application (`index.html`)
* **Interactive UI:** Uses sliders for numerical inputs (Cylinders, Horsepower, etc.) and radio buttons for 'Origin'.
* **Real-Time Prediction:** Instantly calculates and displays the predicted MPG as the user adjusts the sliders.
* **Qualitative Feedback:** The predicted MPG value is color-coded (Poor, Fair, Good, Excellent) for easy interpretation.
* **Preset Examples:** Includes "Quick Example" cards for an Efficient City Car, a Powerful SUV, and a Reliable Sedan to demonstrate the tool.

---

## 📈 Model Performance

The final model selected was the **Random Forest Regressor**, which yielded the best performance on the test set:

* **R² Score:** 0.933
* **Mean Absolute Error (MAE):** 1.516
* **Root Mean Squared Error (RMSE):** 2.074

*Note: The `predictMPG()` function in `index.html` is a simplified JavaScript approximation of the Random Forest model's logic for demonstration purposes.*

---

## 🛠️ Technology Stack

* **Machine Learning:**
    * Python 3
    * Jupyter Notebook
    * Pandas
    * Scikit-learn (for all modeling and preprocessing)
    * Matplotlib & Seaborn (for data visualization)
    * Joblib (for model serialization)

* **Web Application:**
    * HTML5
    * CSS3
    * JavaScript (ES6)
