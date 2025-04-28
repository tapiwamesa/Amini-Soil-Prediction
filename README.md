# Soil Nutrient Prediction for Optimized Maize Yield

## 🌱 Overview
Soil health is fundamental to sustainable agriculture, directly influencing crop yield and food security.  
This project focuses on building a **machine learning model** to predict the availability of **11 essential soil nutrients** and calculate the **nutrient gaps** required for **maize crops** to achieve a **target yield of 4 tons per hectare**.

The model leverages soil and environmental data collected from farms across Africa (2019 dataset) to provide precise fertilizer and soil management recommendations.

By offering scalable and cost-effective soil analysis, this solution empowers farmers to:
- Optimize fertilizer use
- Improve soil management practices
- Maximize crop yields sustainably

## 🔬 Key Features
- Predicts availability of key macronutrients (N, P, K) and micronutrients (Ca, Mg, etc.).
- Calculates nutrient gaps to reach the target maize yield.
- Uses real-world soil and environmental data from African farms.
- Supports data-driven, sustainable agriculture practices.

## 📦 Tech Stack
- **Python** (for model building and analysis)
- **Scikit-learn**, for ML frameworks
- **Pandas** and **NumPy** for data processing
- **Matplotlib** and **Seaborn** for visualization
- **Google Colab** for development and prototyping

  ## 📊 Results
In this project, we developed and evaluated three machine learning models thus Linear Regression, Random Forest, and LightGBM to predict soil nutrient availability and calculate nutrient gaps for optimizing maize yields.

The models were assessed using Mean Squared Error (MSE) and Root Mean Squared Error (RMSE) metrics below:

| Metric       | Linear Regression | Random Forest | LightGBM    | 
|--------------|-------------------|---------------|-------------|
| MSE          |     214.040927    | 159.883897    | 158.057342  | 
| RMSE         |     14.630138     | 12.644520     | 12.572086   | 

- The Linear Regression model showed the highest error, indicating that simple linear relationships were insufficient to capture the complexity of soil nutrient dynamics.
- The Random Forest model significantly reduced the MSE and RMSE compared to Linear Regression, demonstrating that ensemble-based methods better model nonlinear relationships in the data.
- LightGBM achieved the best performance overall, with the lowest MSE (158.06) and RMSE (12.57), suggesting it can most accurately predict soil nutrient levels in this context.

Given its superior accuracy, **LightGBM** is the recommended model for deployment to support soil analysis and fertilizer recommendation systems. Its ability to handle complex feature interactions and large datasets makes it particularly suitable for scaling this solution across diverse agricultural regions.

## 📊 Future Improvements
- Deploy the model as an API for real-time nutrient recommendations.
- Expand to other crops and target yields.
- Integrate with satellite or drone data for enhanced environmental features.

## 🙌 Acknowledgements
Special thanks to Zindi community, the farmers and researchers involved in collecting soil and environmental data across Africa.

---
