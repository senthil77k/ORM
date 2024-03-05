# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Book database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

![diagram](<Screenshot 2024-03-04 102443.png>)
 



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
-Models 
```
from django.db import models
from django.contrib import admin
class Books_DB(models.Model):
    serial=models.IntegerField(primary_key=True);
    title=models.CharField(max_length=20);
    author=models.CharField(max_length=20);
    price=models.IntegerField( );
    genre=models.CharField(max_length=20);
class Books_DBAdmin(admin.ModelAdmin):
    list_display=("serial","title","author","price","genre");
```
-Admin
```
from django.contrib import admin
from .models import Books_DB,Books_DBAdmin 
admin.site.register(Books_DB,Books_DBAdmin)
```

## OUTPUT
![output](Screenshot%202024-03-04%20095843.png)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
