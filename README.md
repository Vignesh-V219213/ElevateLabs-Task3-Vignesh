#  Task 3 - Housing Price Prediction using Linear Regression

##  Dataset Description

The dataset used in this project is the **Housing Price Dataset**, a classic dataset commonly used for regression tasks.  
It contains features related to houses, such as:
- **area**: total area of the house (in square feet),
- **bedrooms**: number of bedrooms,
- **bathrooms**: number of bathrooms,
- **stories**: number of stories,
- **mainroad**: is there a main road access (yes/no),
- **guestroom**: is there a guest room (yes/no),
- **basement**: presence of a basement (yes/no),
- **hotwaterheating**: presence of hot water heating (yes/no),
- **airconditioning**: presence of air conditioning (yes/no),
- **parking**: number of parking spaces,
- **prefarea**: is there a preferred area (yes/no),
- **furnishingstatus**: furnishing status (furnished/semi-furnished/unfurnished),
- **price**: **(target)** price of the house.

---

##  Steps Performed

### 1. Import Libraries and Load Dataset
- Imported libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, and `scikit-learn`.
- Loaded the dataset into a Pandas DataFrame.

### 2. Data Preprocessing
- Checked for missing values and found none.
- Converted categorical variables (like `mainroad`, `guestroom`, `basement`, etc.) into numerical values using **One-Hot Encoding**.
- The target variable (`price`) was separated from feature variables.

### 3. Train-Test Split
- Split the data into training and testing sets with an 80:20 ratio.

### 4. Model Training
- Created a **Linear Regression** model using `LinearRegression()` from `sklearn.linear_model`.
- Trained the model (`fit`) on the training set.

### 5. Model Evaluation
- Made predictions on the test set (`predict`).
- Evaluated model performance using:
  - **Mean Absolute Error (MAE)**: Measures average magnitude of errors.
  - **Mean Squared Error (MSE)**: Penalizes larger errors more.
  - **R² Score**: Measures how well the model explains the variance in the target variable.

### 6. Visualization
- Plotted **Actual Prices vs Predicted Prices** using a scatter plot.

---

##  Coefficient Interpretation

Each feature's coefficient explains its influence on house price:
- A **positive coefficient** suggests that increasing this feature increases the price.
- A **negative coefficient** means an increase in that feature decreases the price.

---
