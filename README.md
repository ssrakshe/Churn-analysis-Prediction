# Churn-analysis-Prediction
Its a project to understand data analytics &amp; strategies<br />
In this repository, we have performed the end to end Exploratory Data Analysis, and idenfitied the characteristics of the customers that are more likely to churn, and I have used them wisely to create a model, and lately, have deployed the model.

🟢 For EDA, please refer to : Churn Analysis - EDA.ipynb<br />
🟢 For Model Building, please refer to: Churn Analysis - Model Building.ipynb<br />
🟢 For Model Deployment, please refer to app.py<br />
🔵 Creating the flask API<br />
app = Flask("__name__")<br />
The loadPage method calls our home.html.<br />

@app.route("/")<br />
def loadPage():<br />
	return render_template('home.html', query="")<br />
The predict method is our POST method, which is basically called when we pass all the inputs from our front end and click SUBMIT.<br />

@app.route("/", methods=['POST'])<br />
def predict():<br />
The run() method of Flask class runs the application on the local development server.<br />

app.run()<br />
Yay, our model is ready, let’s test our bot. The above given Python script is executed from Python shell.<br />


Go to Anaconda Prompt, and run the below query.

python app.py
Below message in Python shell is seen, which indicates that our App is now hosted at http://127.0.0.1:5000/ or localhost:5000

* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
