# Ex02 Django ORM Web Application
## Date: 13/03/2025

## AIM
To develop a Django application to store and retrieve data from a Movies Database using Object Relational Mapping(ORM).


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
```python

admin.py

from django.contrib import admin
from .models import Employee, EmployeeAdmin
admin.site.register(Employee, EmployeeAdmin)

models.py

from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid = models.CharField(max_length=20, help_text="Employee id")
    name = models.CharField(max_length=100)
    salary = models.IntegerField()
    age = models.IntegerField()
    email = models.EmailField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display = ('eid', 'name', 'salary', 'age', 'email')
```


## OUTPUT

![Screenshot 2025-03-11 133603](https://github.com/user-attachments/assets/89aa4c53-0a3e-49be-8137-a9c01765afc6)


## RESULT
Thus the program for creating movies database using ORM hass been executed successfully
