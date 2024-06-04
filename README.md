# AIGS538 Deep Learning Project : Analyzing the Impact of Extracting Representative Data on Deep Learning Model Performance

- Our motivation was to reduce the number of data so that we only use key representative samples during training. We used 5 algorithms to reduce the datasets ; interval mean, k-medoid, k-mean, min-max, and random reduction.
- If you want to run each reduction algorithm, you can run ipynb files below including the name.

### **Code List**

- 딥러닝 interval mean 정리.ipynb
- 딥러닝 k_medoid.ipynb
- 딥러닝 k mean 정리.ipynb
- 딥러닝 max_min.ipynb
- 딥러닝 random reduction.ipynb



### **Description 1**

- K-means, Interval mean code description
- You can change the capacity in **<u>4-3) fixed capacity results</u>**, and the fixed capacity used in this research is 2 layers.
- You can change the number of reduced datasets in <u>**4-2) dataloader with reduced dataset**</u>, and the range of number of datasets is from 3~200.

1. Setting
   - Import Required Libraries
   - Hyperparameters
2. Data
   - Generate data
   - Dataset reduction
     - **(a) reduction algorithm**
       - **: interval mean or kmean**
     - (b) dataloader with reduced dataset
     - (c) plot reduced dataset
3. Training with reduced samples
   - Define model
   - Training
     - (a) Learning curve
     - (b) True Function vs Model Prediction
   - Model Selection
     - (a) Validation curve
4. Results
   - Example
   - Whole result (with optimal capacity)
     - (a) train, evaluate, test whole reduced dataset
     - (b) plot whole reduced dataset
   - Whole result (with fixed capacity = 2)

### **Description 2**

- K-medoid, max-min, random reduction description
- You can change the capacity in **<u>3-2) Training</u>,** # of hidden layer varaible 'i', and the fixed capacity used in this research is 2 layers.
- You can change the number of reduced datasets in **<u>3-2) Training</u>,** argument of training reduction as variable 'num', and the range of number of datasets is from 3~200.
  - In case of random reduction, you have to change # of reduced datasets after 2**-2) Dataset Reduction**, using 'num' variable

1. Settings
   - Import required libraries 
   - Hyperparameters
2. Data
   - Generate data
   - **Dataset reduction**
     - **: K-medoid, min-max, random reduction**
3. Training with reduced samples
   - Define model
   - Training
   - Learning curve
   - True function vs Model Prediction
   - Model selection
   - Results
