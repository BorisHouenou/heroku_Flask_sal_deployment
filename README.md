#Check the all code files in "master" branch

# heroku_Flask_sal_deployment
deploy simple salary prediction model using Flask and deploy in Heroku

Deployed URL in Heroku
https://sal-prediction-flask.herokuapp.com/

## ML-Model-Flask-Deployment

This is a demo project to elaborate how Machine Learn Models are deployed on production using Flask API
Prerequisites

This project has four major parts :

    model.py - This contains code for our ML model to predict employee salaries observed on training data in 'hiring.csv' file.
    app.py - This contains Flask APIs that receives employee details through GUI or API calls, computes the precited value based on our model and returns it.
    request.py - This uses requests module to call APIs already defined in app.py and dispaly the returned value.
    templates -  HTML template to allow user to enter employee detail and displays the predicted employee salary.

Running the project

    I am using Visual studio code to run my project, you can choose your own editor.
   Run the below commands by opening cmd prompt in the same folder, consists of all files
   
python model.py

This would create a serialized version of our model into a file model.pkl

    Run app.py using below command to start Flask API

python app.py

By default, flask will run on port 5000.

    Navigate to URL http://localhost:5000

You should be able to view the homepage as below : alt text



![predict-html](https://user-images.githubusercontent.com/66937023/104154522-1f36f180-540b-11eb-94bf-803bbd47b0f8.PNG)




Enter valid numerical values in all 3 input boxes and hit Predict.

If everything goes well, you should be able to see the predcited salary vaule on the HTML page! alt text

    You can also send direct POST requests to FLask API using Python's inbuilt request module Run the beow command to send the request with some pre-popuated values -

python request.py

