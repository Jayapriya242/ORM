# Ex02 Django ORM Web Application
## Date: 22-03-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![ER-2](https://github.com/Jayapriya242/ORM/assets/114279259/155a5f68-a756-4793-8efe-f2216e8b6c46)




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
model.py
```
from django.db import models
from django.contrib import admin
class Employee (models.Model):
    eid=models.IntegerField(primary_key=True)
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()
 
class EmployeeAdmin(admin.ModelAdmin):
    list_display=('eid','name','salary','age','email')

```
Admin.py

```

from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)


```


## OUTPUT
<img width="960" alt="image" src="https://github.com/Jayapriya242/ORM/assets/114279259/a22043d9-ed12-49f3-8f52-d648167a4828">




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
