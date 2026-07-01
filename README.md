## 🔴 What is Customer Churning ?

![Customer Retention](https://raw.githubusercontent.com/pik1989/MLProject-Churn-Analysis-And-Prediction-Model/main/images/Telco1.JPG)

## 🔴 What are the different Churn Scenarios ?

![Churn Scenarios](https://raw.githubusercontent.com/pik1989/MLProject-Churn-Analysis-And-Prediction-Model/main/images/Telco2.JPG)

## 🔴 Decision Cycle of a Subscriber ?

![Decision Cycle](https://raw.githubusercontent.com/pik1989/MLProject-Churn-Analysis-And-Prediction-Model/main/images/Telco3.JPG)

## 🔴 What are the different Churn Segments ?

![Churn Segments](https://raw.githubusercontent.com/pik1989/MLProject-Churn-Analysis-And-Prediction-Model/main/images/Telco4.JPG)

## 🔴 Solution Overview

![Solution](https://raw.githubusercontent.com/pik1989/MLProject-Churn-Analysis-And-Prediction-Model/main/images/Telco5.JPG)


In this repository, we have performed the end to end Exploratory Data Analysis, and idenfitied the characteristics of the customers that are more likely to churn, and I have used them wisely to create a model, and lately, have deployed the model.

### 🟢 For EDA, please refer to : Churn Analysis - EDA.ipynb
### 🟢 For Model Building, please refer to: Churn Analysis - Model Building.ipynb
### 🟢 For Model Deployment, please refer to app.py


### 🔵 Creating the flask API

```
app = Flask("__name__")
```

The loadPage method calls our home.html.
```
@app.route("/")
def loadPage():
	return render_template('home.html', query="")
```

The predict method is our POST method, which is basically called when we pass all the inputs from our front end and click SUBMIT.
```
@app.route("/", methods=['POST'])
def predict():
```
  
The run() method of Flask class runs the application on the local development server.
```
app.run()
```


Yay, our model is ready, let’s test our bot.
The above given Python script is executed from Python shell.

Go to Anaconda Prompt, and run the below query.
```
python app.py
```


Below message in Python shell is seen, which indicates that our App is now hosted at http://127.0.0.1:5000/ or localhost:5000
```
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```


HERE'S HOW OUR FRONTEND LOOKS LIKE:

![Customer Retention](https://raw.githubusercontent.com/pik1989/MLProject-Churn-Analysis-And-Prediction-Model/main/images/Telco6.JPG)

# 📊 Customer Churn Prediction

A Machine Learning project that predicts whether a customer is likely to churn based on demographic and service-related information. The project includes data analysis, model building, and a web interface for real-time predictions.

---

## 🚀 Features

- Customer churn prediction using Machine Learning
- Exploratory Data Analysis (EDA)
- Data preprocessing and feature engineering
- Model training and evaluation
- Real-time prediction using Flask
- User-friendly web interface

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Flask
- HTML
- CSS

---

## 📂 Project Structure

```
Customer-Churn-Prediction/
│
├── app.py
├── model.pkl
├── templates/
│   └── home.html
├── static/
├── Churn Analysis - EDA.ipynb
├── Churn Analysis - Model Building.ipynb
├── requirements.txt
└── README.md
```

---

## ⚙️ Workflow

1. Load customer dataset.
2. Perform Exploratory Data Analysis (EDA).
3. Clean and preprocess the data.
4. Train and evaluate the Machine Learning model.
5. Save the trained model.
6. Deploy the model using Flask.
7. Predict customer churn through a web interface.

---

## 📈 Model Pipeline

```
Customer Data
      ↓
Data Preprocessing
      ↓
Exploratory Data Analysis
      ↓
Feature Engineering
      ↓
Model Training
      ↓
Model Evaluation
      ↓
Flask Deployment
      ↓
Customer Churn Prediction
```

---

## 📦 Installation

```bash
git clone <repository-url>
cd Customer-Churn-Prediction
pip install -r requirements.txt
```

---

## ▶️ Run

```bash
python app.py
```

Open your browser and visit:

```
http://127.0.0.1:5000/
```

---

## 🎯 Future Enhancements

- Improve prediction accuracy
- Deploy on Render or Railway
- Add authentication
- Interactive dashboard
- Real-time analytics

---

## 🙏 Acknowledgements

This project was developed for learning purposes by exploring customer churn prediction concepts and implementing an end-to-end machine learning workflow.

---

## 📄 License

This project is intended for learning and educational purposes.
