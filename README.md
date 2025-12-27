# Ex01 Django ORM Web Application
## Date:28-11-2025 

## AIM
To develop a Django application to store and retrieve data from a Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 10 books

## PROGRAM

Models.py

from django.db import models
from django.contrib import admin

class Employee(models.Model):
    eid = models.CharField(max_length=20, help_text="Employee ID")
    name = models.CharField(max_length=100)
    salary = models.IntegerField()
    age = models.IntegerField()
    email = models.EmailField()

    
admin.py

from Django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee, EmployeeAdmin)

cd projectname
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
python manage.py makemigrations ormapp
python manage.py migrate ormapp
python manage.py runserver

## OUTPUT
<img width="1920" height="1080" alt="Screenshot_2025-12-27_21_30_12" src="https://github.com/user-attachments/assets/42269497-4fcf-4f92-85b5-a2c74ed56594" />




## RESULT
Thus the program for creating car inventory database database using ORM hass been executed successfully
