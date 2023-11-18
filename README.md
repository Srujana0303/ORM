# Ex02 Django ORM Web Application
## Date: 07-10-23

## AIM
To develop a Django application to store and retrieve data from a Football Players database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create 10 Football players

## PROGRAM

```py
Models.py

from django.db import models
from django.contrib import admin
class Player (models.Model):
    p_id=models.CharField(max_length=20,help_text="PlayerID")
    name=models.CharField(max_length=100)
    salary=models.IntegerField()
    age=models.IntegerField()
    email=models.EmailField()

class PlayerAdmin(admin.ModelAdmin):
    list_display=('p_id','name','salary','age','email')



Admin.py

from django.contrib import admin
from .models import Player,PlayerAdmin
admin.site.register(Player,PlayerAdmin)
```

## OUTPUT
![image](https://github.com/Srujana0303/ORM/assets/132996836/a178509b-58de-42dd-9d5a-c7b99a0df193)


![image-1](https://github.com/Srujana0303/ORM/assets/132996836/36b08a9d-3ec1-4a37-a8d8-be223ad540e3)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
