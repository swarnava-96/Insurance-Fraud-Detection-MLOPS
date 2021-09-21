# Insurance-Fraud-Detection-MLOPS

## Goal: To build a classification methodology to determine whether a customer is placing a fraudulent vehicle insurance claim.

## About the Data set:
The data was sent from the client side in multiple sets of files in batches at a given location. The data has been extracted from the census bureau. The Dataset has 38 features(including the target feature).

## Project Description:
Schema file was also sent by the client containing the relevent informations about training files. Data Validation was performed as an initial step followed by data insertion into Database(SQLite). Here data is divided into good and bad data based on the schema file and then sent to respective folders. Then the entire lifecycle of a Data Science project was followed like, exporting data from database,data preprocessing(Imbalanced dataset was handled using Imblearn's Random Over sampler),clustering using Kmeans,model selection(multiple models were tested and the top 2 models were selected based on accuracy score and AUC score), model building(XgBoost for the first cluster and SVC for the second), hyperparameter optimization(using GridSearchCV) and finally model deployment(into GCP). API testing was done using Postman. Logs were maintained at each and every step of action. Similar set of actions were performed for the predicting data. Codes were written following OOPS concept.

For more details about the project click [here](https://github.com/swarnava-96/Insurance-Fraud-Detection-MLOPS/blob/main/documentation/Project%20Documentation.pdf)

## Project Architecture:

![image](https://user-images.githubusercontent.com/75041273/129022437-05b6056a-8943-47d3-a4a3-da17acfbb9e3.png)

## Installation:
The Code is written in Python 3.7.3 If you don't have Python installed you can find it [here](https://www.python.org/downloads/). If you are using a lower version of Python you can upgrade using the pip package, ensuring you have the latest version of pip. To install the required packages and libraries, run this command in the project directory after [cloning](https://www.howtogeek.com/451360/how-to-clone-a-github-repository/) the repository:

##### 1. First create a virtual environment by using this command:
```bash
conda create -n myenv python=3.7
```
##### 2. Activate the environment using the below command:
```bash
conda activate myenv
```
##### 3. Then install all the packages by using the following command
```bash
pip install -r requirements.txt
```
##### 4. Then, in cmd or Anaconda prompt write the following code:
```bash
python main.py
```
##### Make sure to change the directory to the root folder.  

## Deployment on GCP
Login or sign up in order to create virtual app and many more things. Free tier account on Google console provides $300 credit for one year. For application deployment download the Google SDK installer.

## Frontend using HTML and Backend using Flask:

https://insurancefraud.de.r.appspot.com/

![Screenshot (99)](https://user-images.githubusercontent.com/75041273/129017508-18e3b8ac-c08f-4fce-9e3f-b10bcf8e41a3.png)
![Screenshot (100)](https://user-images.githubusercontent.com/75041273/129017696-327f347f-1ea1-49e0-90f3-e21c1067374f.png)

Currently app disabled,since GCP is chargeable.
![Screenshot (101)](https://user-images.githubusercontent.com/75041273/129017832-1db713d3-03f4-4089-a0b7-e14aec71f210.png)

## Technology Stack:

![](https://forthebadge.com/images/badges/made-with-python.svg)

![PyCharm](https://img.shields.io/badge/pycharm-143?style=for-the-badge&logo=pycharm&logoColor=black&color=black&labelColor=green) <img src="https://img.shields.io/badge/Numpy-777BB4?style=for-the-badge&logo=numpy&logoColor=white" /> <img src="https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white" /> <img src="https://img.shields.io/badge/scikit_learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" /> <img src="https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white" /> <img src="https://img.shields.io/badge/conda-342B029.svg?&style=for-the-badge&logo=anaconda&logoColor=white"/> ![SciPy](https://img.shields.io/badge/SciPy-%230C55A5.svg?style=for-the-badge&logo=scipy&logoColor=%white) ![Seaborn](https://img.shields.io/badge/Seaborn-%230C55A5.svg?style=for-the-badge&logo=seaborn&logoColor=%white) <img src="https://img.shields.io/badge/matplotlib-342B029.svg?&style=for-the-badge&logo=matplotlib&logoColor=white"/> <img src="https://img.shields.io/badge/Stack_Overflow-FE7A16?style=for-the-badge&logo=stack-overflow&logoColor=white" /> <img src="https://img.shields.io/badge/HTML-239120?style=for-the-badge&logo=html5&logoColor=white" /> <img src="https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white" /> <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" /> <img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=Postman&logoColor=white"/> <img src="https://img.shields.io/badge/Google_Cloud-4285F4?style=for-the-badge&logo=google-cloud&logoColor=white" />

## Further Changes to be Done:

- [ ] Deploying the Web Application on Cloud.
     - [ ] Heroku
     - [ ] Azure
     - [ ] AWS EC2 Instance

