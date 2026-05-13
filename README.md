# Ex01 Django ORM Web Application
## Date: 2/5/2026

## AIM
To develop a Django Application to store and retrieve data from an Online Food Delivery Database platform like Zomato or Swiggy using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

<img width="916" height="526" alt="{B6BD2335-799D-458B-8B9C-CBD3C5B6CF5B}" src="https://github.com/user-attachments/assets/00ddf656-62f8-460d-a1b2-1467acaea93d" />


## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py


### STEP 4:
Detect changes and create migration files that describe how to modify the database schema

### STEP 5:
Execute the migration files and update the database schema to match your Django models

### STEP 6:
Create a superuser with full access rights to all models and data through the admin interface.

### STEP 7:
Apply the migration files of the created app to the database

### STEP 8:
Execute Django admin using localhost and create details for 10 entries

## PROGRAM

```
admin.py

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)


models.py

from django.db import models
from django.contrib import admin

class Employee (models.Model):
    eid=models.CharField(max_length=20,help_text="Employee_ID")
    name = models.CharField(max_length=100)
    salary = models.IntegerField()
    age = models.IntegerField()
    email = models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

```


## OUTPUT
<img width="1045" height="487" alt="{94425086-930C-48AE-B6CD-F537DF729B51}" src="https://github.com/user-attachments/assets/4e08dc04-c052-4680-8151-89cdbc822ded" />


## RESULT
Thus the program for creating Online Food Delivery Database using ORM hass been executed successfully
