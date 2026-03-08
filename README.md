# 📦 E-Commerce Logistics & Delivery Prediction

## 📌 Business Objective
Late deliveries in e-commerce directly impact customer satisfaction and increase support costs. This project aims to predict whether a shipment will be delayed (Class 1) based on logistics data (weight, warehouse, shipping mode, discounts) so the business can act proactively.

## 🛠️ Tools & Technologies
* **Language:** Python
* **Data Manipulation & Cleaning:** Pandas, NumPy
* **Machine Learning:** Scikit-Learn, XGBoost
* **Data Visualization:** Matplotlib, Seaborn

## 🧠 The Approach
1. **Data Cleaning & Engineering:** Removed non-predictive features (IDs) and converted categorical text data (like "Flight" or "Ship") into binary numeric columns using One-Hot Encoding.
2. **Feature Scaling:** Applied `StandardScaler` to balance the mathematical weights of distinct variables like product cost and weight in grams.
3. **Model Evaluation & Tuning:** Tested multiple algorithms from baseline (k-NN, SVM) to advanced ensemble methods (Random Forest, Gradient Boosting, XGBoost), including Hyperparameter Tuning via `GridSearchCV`.

## 🏆 Business Results & Insights
During exploratory analysis, an unexpected business insight emerged: **Air freight (Flight) had the highest delay rate (~60%)** compared to Road and Ship.

On the predictive side, even after rigorous hyperparameter tuning, the models hit a performance ceiling:
* **Best Accuracy:** ~67%
* **Best Recall (Late Deliveries):** ~65%

**Executive Conclusion:** The current dataset lacks critical external variables that heavily influence logistics (e.g., weather conditions, port strikes, mechanical failures). A 67% accuracy proves that the available internal variables alone are insufficient to fully explain supply chain delays.

## 🚀 Next Steps
* Transition from Machine Learning to Business Intelligence.
* Develop an operational Power BI dashboard to monitor bottlenecks, visualize delays by shipping mode, and enable data-driven decision-making for the logistics team.
