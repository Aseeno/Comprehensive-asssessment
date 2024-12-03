Diabetes Progression Modeling
Objective
This project models the progression of diabetes using independent variables from the Diabetes dataset in the sklearn library. The objective is to help healthcare professionals understand the factors influencing diabetes progression, enabling better treatment planning and prevention strategies.

Dataset
The Diabetes dataset contains 10 baseline variables (age, BMI, blood pressure, etc.) and a target variable representing disease progression one year after baseline measurements.

Features: 10 numerical variables.
Target: Disease progression score.
Key Components
1. Loading and Preprocessing
Loaded the dataset using sklearn.datasets.load_diabetes.
Verified there were no missing values.
Normalized the features using StandardScaler to improve model performance.
2. Exploratory Data Analysis (EDA)
Analyzed the distribution of features and the target variable.
Visualized relationships between features and the target variable using scatter plots and pair plots.
3. Building the Artificial Neural Network (ANN)
Designed a simple ANN model with the following architecture:
Input Layer: 10 nodes (features).
Hidden Layer 1: 64 neurons, ReLU activation.
Hidden Layer 2: 32 neurons, ReLU activation.
Output Layer: 1 neuron for regression.
Used the Adam optimizer and Mean Squared Error loss function.
4. Training the ANN Model
Split the data into training and testing sets (80% train, 20% test).
Trained the model for 50 epochs with a batch size of 16.
5. Evaluating the Model
Evaluated the model using:
Mean Squared Error (MSE): Measures average squared difference between predicted and actual values.
R² Score: Indicates how well the model explains variance in the target variable.
6. Improving the Model
Experimented with the following changes:
Increased the number of hidden layers and neurons.
Added different activation functions like tanh.
Tuned the learning rate and batch size.
Observed improved performance metrics after adjustments.
Results
Metric	Initial Model	Improved Model
MSE	3100	2800
R² Score	0.45	0.50
   
   











