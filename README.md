# Django_first_project
This project is a chatroom  build with Django  
I followed this tutorial to build the project : [Python Django 7 Hour Course](https://www.youtube.com/watch?v=PtQiiknWUcI&t=13201s). 
And Thanks to it I had a good understanding about Django basics.  
It was a great starting point for me !
### Project Description
This chatroom I used :
  - **Django :** for the backend 
  - **Django templates:** for the frontend
  - **sqlite :** the Databse 

For the template I integrated a free theme used in the tutorial. 
### How can I run the project ?
First you must have python installed
After downloading the project, go to the directory and run this command to install django :
```
pip install -r requirements.txt
```
After, to launch the project Just run:
```
python manage.py runserver
```
### Some notes :
As i said while building this project I uderstood some of the basics of Django.  
#### Creating a new app :
Django has a unique structure. It divides the projects to independant apps.   
To create a new app run :
```
python manage.py startapp YOUR_APP_NAME
```
Then, a new directory for this app will be  created.

#### Models :
Models are python calsses that represents the database tables. Every single attribute in teh classe will represent a column.   
To crate a model class you should first import Model class from django.db.models and each new model class should extend this class.  
Migration : After modifying our models we should run these two commands :
```
Python manage.py makemigrations
```
This command transforms the model classes into SQL commands to be executed
```
Python manage.py migrate
```
This command executes the SQL commands to the database
#### Views :
In Django, views are python functions that hundles the Http requests and returns a response .
> :warning: **Do not get confused with the views with other MVC frameworks**: Django follows the MVT pattern where the view (V) cooresponds to the controller in the mvc and the templates (T) corresponds to the views !
