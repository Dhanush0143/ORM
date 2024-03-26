# Ex02 Django ORM Web Application
## Date:28.02.2024

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![WhatsApp Image 2024-03-26 at 11 34 47_d29af6f1-1](https://github.com/Dhanush0143/ORM/assets/139841924/f151b2e0-1137-4676-9dad-3f69e1185b97)

 
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

```
models.py
from django.db import models
from django.contrib import admin
class libraryBook(models. Model):
    title=models.CharField(max_length=15);
    BookID=models.IntegerField(primary_key=True);
    author=models.CharField(max_length=10);
    publisher=models.CharField(max_length=8);
    price=models.IntegerField();
    pages=models.IntegerField();
class libraryBookAdmin(admin.ModelAdmin):
   list_display=("title","BookID","author","publisher","price","pages");

admin.py
from django.contrib import admin 
from .models import libraryBook,libraryBookAdmin
admin.site.register(libraryBook,libraryBookAdmin)
```
## OUTPUT
![Screenshot 2024-03-26 112759-1-1](https://github.com/Dhanush0143/ORM/assets/139841924/e90315c3-d6d7-4da7-904c-543e3f8a89c3)

 


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
