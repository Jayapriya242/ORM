# Ex02 Django ORM Web Application
## Date: 21-03-2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here
![WhatsApp Image 2024-03-21 at 22 49 50_5c1eeb87](https://github.com/Jayapriya242/ORM/assets/114279259/8f0d2e77-66eb-4046-bba1-fc36b99b70e4)



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
models.py
```
 from django.db import models
 from django.contrib import admin
 class Book(models.Model):
 bookno=models.IntegerField(primary_key="bookno")
 bookname=models.CharField(max_length=20)
 authorname=models.CharField(max_length=40)
 publishdate=models.DateField()
 price=models.IntegerField()
 class BookAdmin(admin.ModelAdmin):
 list_display=("bookno", "bookname", "authorname", "publishdate","price"
```
 admin.py
 ```
 from django.contrib import admin
 from .models import Book,BookAdmin
 admin.site.register(Book,BookAdmin)
```


## OUTPUT
![WhatsApp Image 2024-03-21 at 22 50 29_7735afcb](https://github.com/Jayapriya242/ORM/assets/114279259/5ec9bbbd-0ee0-4655-8ef8-7c027e8ca167)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
