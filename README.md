# House Price Prediction using Linear Regression

This project implements **Simple** and **Multiple Linear Regression** using the `scikit-learn` library to predict house prices based on various features such as area, bedrooms, location, and amenities.

---

## Dataset Description

The dataset contains information on houses and their attributes:

| Feature            | Description                                     |
|--------------------|-------------------------------------------------|
| `Price`            | Price of the house                              |
| `Area`             | Area in square feet                             |
| `Bedrooms`         | Number of bedrooms                              |
| `Bathrooms`        | Number of bathrooms                             |
| `Stories`          | Number of floors                                |
| `Mainroad`         | Connected to main road (Yes/No)                 |
| `Guestroom`        | Has guestroom (Yes/No)                          |
| `Basement`         | Has basement (Yes/No)                           |
| `Hotwaterheating`  | Has hot water heating (Yes/No)                 |
| `Airconditioning`  | Has air conditioning (Yes/No)                  |
| `Parking`          | Number of parking spaces                        |
| `Prefarea`         | Preferred area (Yes/No)                         |
| `Furnishing Status`| Fully, Semi or Unfurnished                      |

---

## 🔧 Tools Used

- **Python 3**
- **pandas** for data handling
- **scikit-learn** for model building
- **matplotlib** for visualization

---
##Tasks Performed
🔹 Data Preprocessing
Converted binary categorical variables (Yes/No → 1/0)

Encoded Furnishing Status using one-hot encoding

Handled missing values (if any)

🔹 Simple Linear Regression
Used Area to predict Price

Plotted regression line

🔹 Multiple Linear Regression
Used all relevant features

Evaluated using:

MAE (Mean Absolute Error)

MSE (Mean Squared Error)

R² Score

🔹 Visualization
Plotted Actual vs Predicted prices

(Optional) Residual plots

📈 Sample Output
Evaluation Metrics (Multiple Linear Regression):

MAE: ~970,000

MSE: ~1.75e+12

R² Score: ~0.65

📊 Interpretation of Results
R² Score ~0.65 indicates that about 65% of the variance in house prices is explained by the model. While not perfect, it's a reasonably good fit for real-world data.

MAE (~970k) and MSE (~1.75e+12) suggest that there is still a significant error in absolute and squared terms. MAE gives an average deviation of nearly ₹9.7 lakhs.

The Actual vs Predicted scatter plot shows that most points are fairly close to the red line (ideal prediction), but there is some scatter—especially at higher prices. This means the model is reasonably accurate, but errors increase for high-priced houses.
