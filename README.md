# ML_visualizer

Here I used streamlit to visualize a dataset, perform some quary on it, and finally train a machine learning model using sklearn. Finally I plotted some basic curve like ROC-AUC, Precision-Recall and confusion matrix on fly.    
All instruction are provided here      
    
### Dataset 
+ Dataset can also be founf from *[here](https://archive.ics.uci.edu/ml/datasets/Mushroom)*    

## Instruction to run 
+ change the line no 20 in app.py to provide the data path
+ open cmd
+ cd over the **ML_visualizer**
+ to install depencies `pip install -r requirements.txt`
+ run the command `streamlit run app.py`    
+ hopefully it is running on `http://localhost:8501`

## Hosting process
### To make it available on cloud for free(heroku)
1.  install git on your system, if not already present. Then run these 3 command in cmd    
`git init`    
`git add .`    
`git commit -m "Initial commit"`    
2.  install heroku exe and run these line in cmd    
`heroku login`    
`heroku create`    
`git push heroku master`    
`heroku ps:scale web=1`    
`heroku open`   

after heroku login command, login in the browser window if it opens. Hopefully, after completing the above steps your app is successfully deployed and running.    
NOTE : if you are deploying your web app on the cloud (not local machine), you may encounter wrong values of time shown in the raw data in date-time column (more details *[here](https://github.com/streamlit/streamlit/issues/1346)*)

