# Ex02 Django ORM Web Application
## Date: 

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM:
## models.py:
```
from django.db import models
from django.contrib import admin
class Player(models.Model):
    Player_Name=models.CharField(max_length=50)
    Jersy_No=models.IntegerField()
    Team=models.CharField(max_length=20)
    Height=models.IntegerField()
    Position=models.CharField(max_length=100)

class Player_Admin(admin.ModelAdmin):
    list_display=('Player_Name','Jersy_No','Team','Height','Position')
```
## admin.py:
```
from django.contrib import admin
from .models import Player,Player_Admin
admin.site.register(Player,Player_Admin)
```

## OUTPUT

<img width="612" alt="image" src="https://github.com/Srujana0303/ORM/assets/132996836/8ae1a6ad-bce7-4cd5-9cef-f7a2fa297d82">


<img width="609" alt="image" src="https://github.com/Srujana0303/ORM/assets/132996836/e93fea66-6c66-48d1-a5c9-bb4e9722eeb4">



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
