# K-Nearest Neighbors (KNN) Classification on Telecom Dataset

This project demonstrates the classification of customers into categories (`custcat`) based on their demographic and socioeconomic characteristics using the **K-Nearest Neighbors (KNN)** algorithm with a sample dataset called `teleCust1000t.csv`.

## 📊 Dataset
The dataset `teleCust1000t.csv` contains the following features:
- **region**: Customer region (numeric)
- **tenure**: Years as a customer
- **age**: Age of customer
- **marital**: Marital status (0 = single, 1 = married) 
- **address**: Number of years at current address 
- **income**: Annual income 
- **ed**: Education level 
- **employ**: Years employed 
- **retire**: Retired status (0/1) 
- **gender**: Gender (0 = female, 1 = male) 
- **reside**: Number of residents in household

Target Variable: 
- **custcat**: Customer category (1-4)

## ⚙️ Steps
1. **Data Loading and Exploration**
   - Use the `pandas` library to load the dataset.
   - Visualize the feature distributions for each of the customer categories. Also, visualize the counts of each category of customer.

2. **Features Preparation**
- Select relevant features 
- Use `StandardScaler` to normalize the data 

3. **Train/Test Split** 
- Split data into train and test datasets (80% train, 20% test).

4. **Training Model** 
- Train KNN classifier with various values of **K**.

5. **Predictions and Evaluation** 
- Predict customer segments on the test data. 
- Evaluate the accuracy of your predictions using the function `sklearn.metrics.accuracy_score`.

6. **HyperparameterTuning** 
- Run predictions for multiple values of K (K=1-10) 
- Create a plot for accuracy vs. the value of K to determine the optimal K neighbors.

## 📈 Results
- Displays the accuracy for training and test sets.
- Visualization shows the accuracy of different **K** values of this model.
- Displays the **best K value** and its respective accuracy.

## 🛠️ Requirements
Ensure that you have the following Python libraries installed:
