# Credit Card Fraud Detection

## Table of contents
1. [Description](#description)
2. [Dataset](#dataset)
3. [Results](#results)
4. [Steps taken in this Project](#project-steps)
5. [Installation and Usage](#installation-usage)

## Description <a name="description"></a>
A machine learning project on an imbalanced credit card data that detects fraudulent transactions. Out of the whole dataset, only 0.17% of the transactions
were fraudulent. This makes it very hard to detect the outliers in the data with a good accuracy. I visualized certain aspects of the dataset to gain any useful insight. Due to long time of training the models, I used only 20% of the data to train and test our model.

Given below is an easy explanation of credit card fraud detection:
![](images/flowchart.png)  

## Dataset <a name="dataset"></a>
Link of the dataset is in the jupyter notebook

## Results <a name="results"></a>
I used 5 classification algorithms. The key point was not to gain high overall accuracy but high accuracy for only outlier detection because we have to prevent fraudulent transactions not the valid ones. At first it was very difficult to choose certain model for high accuracy. However, I thought of using ensemble model - *Random Forests* and got the outlier's accuracy to be **81%**. I also used an unsupervised algorithm which is used for the sole purpose of anomaly detection - *Isolation Forests* and it performed well on 20% of the dataset. I could choose either of these models for prediction but chose random forest and saved it using pickle.

## Steps taken in this Project <a name="project-steps"></a>
- Data collection
- EDA & visualization
- Model selection & building it
- Evaluation of the models
- Saving the models

## Installation and Usage <a name="installation-usage"></a>
- Requirements:
   - `python >= 3.4`
- `git clone https://github.com/AI-14/credit-card-fraud-detection.git` - clones the repository
- `cd credit-card-fraud-detection`
- `py -m venv yourVenvName` - creates a virtual environment
- `yourVenvName\Scripts\activate.bat` - activates the virtual environment
- `pip install -r requirements.txt` - installs all modules
