# Flight-Price-Prediction-EDA
Exploratory Data Analysis (EDA) of a Flight Price Prediction dataset.

## 📌 Overview
This project performs **Exploratory Data Analysis (EDA)** and **Feature Engineering** on an airline flight dataset to prepare it for **machine learning models** that predict flight ticket prices.

The dataset contains various details about flights such as **Airline**, **Source**, **Destination**, **Duration**, **Total Stops**, and more.  
The goal is to clean, transform, and visualize the data so it can be used for predictive modeling.

## 📂 Dataset Information
The dataset contains the following key features:

1. **Airline** - Name of the airline.
2. **Flight** - Flight code/number.
3. **Source City** - Origin city of the flight.
4. **Departure Time** - Time of departure (converted into hour/minute format).
5. **Stops** - Number of stops (non-stop, 1 stop, 2 stops, etc.).
6. **Arrival Time** - Time of arrival (converted into hour/minute format).
7. **Destination City** - Final location where the flight lands.
8. **Class** - Travel class (Economy or Business).
9. **Duration** - Total travel time in hours/minutes.
10. **Days Left** - Days between booking date and travel date.
11. **Price** - Ticket price (Target Variable).


## 🛠 Steps Performed
### 1. **Importing Required Libraries**
- `pandas`, `numpy` for data handling
- `matplotlib`, `seaborn` for visualization
- `sklearn.preprocessing.OneHotEncoder` for encoding categorical features

### 2. **Data Cleaning**
- Converted **Date_of_Journey** into `Date`, `Month`, `Year`.
- Processed **Duration** into numerical hours and minutes.
- Extracted **Arrival_hour**, **Arrival_min**, **Departure_hour**, **Departure_min`.
- Converted **Total_Stops** into numerical format (non-stop → 0, 1 stop → 1, etc.).
- Handled missing values (NaN) appropriately.

### 3. **Feature Engineering**
- Created new features like:
  - `Days Left` till flight
  - Time-related columns for **Departure** and **Arrival**
- Applied **One-Hot Encoding** to categorical features (`Airline`, `Source`, `Destination`, etc.)

### 4. **Exploratory Data Analysis**
- Visualized:
  - Price distribution per airline
  - Flight duration vs price
  - Impact of stops on price
  - Seasonal/monthly price variations

---

## 📊 Example Visualizations
- Bar plots showing airline average prices.
- Box plots comparing price vs number of stops.
- Heatmap for feature correlations.

---

## 📦 Installation & Requirements

Make sure you have **Python 3.8+** installed.  
Install the required dependencies using:
pip install pandas numpy matplotlib seaborn scikit-learn openpyxl


---

## ▶ How to Run
1. Clone this repository or download the notebook.
2. Install dependencies.
3. Open the Jupyter Notebook:


jupyter notebook 2.0-EDA-And-FE-Flight-Price.ipynb

4. Run all cells to:
- Clean and preprocess the dataset.
- Generate visualizations.
- Get a final machine-learning-ready dataset.



## 📌 Next Steps
- Train machine learning models (e.g., Random Forest, XGBoost, Linear Regression) on the processed dataset.
- Evaluate model performance with metrics like RMSE, R², MAE.
- Tune hyperparameters for better prediction accuracy.



## ✍ Author
 Mukesh Raj
