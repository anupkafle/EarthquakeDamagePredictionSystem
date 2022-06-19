# AI BASED EARHTHQUAKE DAMAGE PREDICTION SYSTEM
The project "Earthquake Damage Prediction System" is a Machine learning project developed using Azure technologies like ML studio for Microsoft Virtual Hackathon 2022. This system is developed with aim to predict damage of buildings due to eathquake. Currently, our models have been trained and tested using only Nepali earthquake dataset taken from Kaggle.com <a href="https://www.kaggle.com/code/ar89dsl/predicting-building-damage-from-earthquakes/data?select=csv_building_structure.csv"> Dataset </a>. Our system can currently predict the earthquake damage grades on buildings with test f1-score of 88%. We have developed this system with two modes of input i-e normal user mode and professional user mode. Here a normal user will enter his/her building id and then get the damage grade predicted for that id. Similarly, the professional user will have to enter some more details of the building like number of floors, height of building, age etc and then get the damage grade predicted for that building. <br>
<b>P.S:<i> Our system is not perfect and this is just a simple prototype for the idea we presented in this hackathon</i></b><br>  

## Want to Use?
You can clone this branch and use it right now using the methods given below.  

## Building
It is best to use python **virtualenv** tool to build locally and use Python 3.8.5:  
> virtualenv venv  
> source venv/bin/activate  
> git clone https://github.com/anupkafle/EarthquakeDamagePredictionSystem.git

Then you navigate to the base directory of the project and install the requirements in your vitual environment  
> pip install -r requirements.txt  

Then you will need to download the dataset and our model link:  
Dataset: [Dataset Link](https://drive.google.com/file/d/1--BBvwc3nOxMW6oE9nkOFk6fhXpolHv6/view?usp=sharing)  
Pre-trained Model: [Model Training Link](https://drive.google.com/file/d/1aWRfPs5901mgWIhz_ETmwSYFuWXJkvdW/view?usp=sharing)  

Then copy the dataset and model file into earthquake>packages  

And finally you make migration to the database, create a super user, and run the server  
> python manage.py makemigrations  
>python manage.py migrate  
> python manage.py createsuperuser  
> python manage.py runserver  

You can predict the house grade as **_normaluser_** and also as **_profesionaluser_**
