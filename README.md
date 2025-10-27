# Understanding and Predicting the Behavioural Pattern of Actuators in a Smart Greenhouse

## Overview
This project explores the behavioral patterns of actuators—such as watering pumps and fans—in a smart greenhouse system. 
The goal is to predict actuator responses based on environmental conditions, improving automation efficiency and energy management.

## Objectives
- Predict when the watering pump should turn on or off using key environmental features.  
- Predict when the fan actuator should activate based on rising temperature levels.  
- Optimize energy and water usage through intelligent automation.

## Data Description
The dataset (`IoTProcessed_Data.csv`) contains 37,922 records with environmental and actuator variables, including:
- Temperature (°C)
- Humidity (%)
- Water Level (%)
- Soil Nutrients:Nitrogen (N), Phosphorus (P), Potassium (K)
- Actuator States: Indicators for ON/OFF status of fans and pumps

## Methodology
1. Data Preparation: 
   - Cleaned and standardized environmental variables.  
   - Corrected column naming inconsistencies.  
   - Scaled features for model readiness.  
2. Modeling:  
   - Watering Pump: Random Forest Classifier (`n_estimators=4`, `max_depth=3`, `criterion='entropy'`)  
   - Fan Actuator: Logistic Regression (`random_state=0`)  
3. Evaluation Metrics:
   - F1 Score  
   - Confusion Matrix Visualization

## Results
Both models achieved near-perfect predictive accuracy:
- Watering Pump Model:
  - Train F1 Score: 0.9999  
  - Test F1 Score: 1.0  
- Fan Actuator Model:
  - Train F1 Score: 0.9998  
  - Test F1 Score: 1.0  

These results show strong predictive power and reliability in modeling actuator behavior.

## Conclusion
The developed models effectively capture actuator response patterns in a greenhouse environment. 
By leveraging environmental data, the system enables smarter automation and more sustainable resource management. 
These insights can guide future work in IoT-driven agriculture and smart environmental systems.

## Tools and Libraries
`Python`, `Pandas`, `NumPy`, `Scikit-learn`, `Seaborn`, `Matplotlib`, `Plotly`
