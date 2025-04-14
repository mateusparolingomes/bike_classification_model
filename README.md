# 🚲 Seoul Bike Demand Classification  

This project analyzes and classifies bike rental demand in Seoul using historical environmental and seasonal data. By leveraging machine learning classification models, we identify key patterns that help predict high versus low demand days, supporting smarter planning and resource allocation.

## 📊 Dataset

- **Source**: UCI Machine Learning Repository  
- **Data**: [Seoul Bike Sharing Demand Data](https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand)  
- **Features**: 14 variables including temperature, humidity, wind speed, precipitation, and season  
- **Target**: High vs Low bike rental demand (derived from 'Rented Bike Count')

## 🧠 Models Used

The following models were trained and evaluated:

- Decision Tree (with hyperparameter tuning: `max_depth`, `min_weight_fraction_leaf`, `min_impurity_decrease`)
- Bagging Classifier
- Boosting Classifier
- XGBoost Classifier
- Neural Network

## 🏆 Results

| Model              | Accuracy |
|-------------------|----------|
| XGBoost           | 93.3%    |
| Neural Network    | 92.5%    |
| Tuned Decision Tree | ~92%  |

## 🔍 Key Insights

- **Environmental factors**: Higher temperature, solar radiation, and dew point positively correlate with high rental demand.
- **Weather**: Rain, snowfall, and high humidity significantly reduce demand.
- **Seasonality**: Spring and summer months see the highest rental activity.
- **Day of the Week**: Weekdays show different rental patterns compared to weekends.

## 💡 Business Recommendations

- **Proactive Resource Allocation**: Use the XGBoost model to forecast demand and prepare bike redistribution ahead of time.
- **Weather-Responsive Strategy**: On low-demand forecast days (rain/snow), optimize for maintenance or reduced operations.
- **Seasonal Campaigns**: Promote special offers during spring/summer when demand peaks.
- **Operational Planning**: Use predictions to support staffing, maintenance scheduling, and customer experience.


## ⚙️ Tools & Technologies

- Python
- Pandas, NumPy
- Scikit-learn
- XGBoost
- Matplotlib, Seaborn

## ✍️ Author

Mateus Parolin Gomes  
Master in Business Analytics @ Hult International Business School  
[GitHub](https://github.com/mateusparolingomes) | [LinkedIn](https://www.linkedin.com/in/mateusparolingomes/)

