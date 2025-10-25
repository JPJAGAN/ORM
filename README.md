# Ex02 Django ORM Web Application
# NAME: JAGAN JP
# REG.NO: 212224230099
## AIM
To develop a Django application to store and retrieve data from Car Inventory Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

<img width="941" height="503" alt="Screenshot 2025-10-23 101327" src="https://github.com/user-attachments/assets/7d4ed69c-191b-4a4e-844e-3f36a040ce9d" />

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
models.py :
from django.db import models

class CAR(models.Model):
    car_id = models.AutoField(primary_key=True)
    brand = models.CharField(max_length=20)
    model = models.CharField(max_length=20)
    year = models.DateField()
    price = models.IntegerField()


admin.py:
from django.contrib import admin
from . models import CAR


# Register your models here.
admin.site.register(CAR)

class CarAdmin(admin.ModelAdmin):
    list_display=('car_id','brand','model','year','price')

```

## OUTPUT

<img width="1546" height="919" alt="Screenshot 2025-10-23 101359" src="https://github.com/user-attachments/assets/0b2f5e2e-f8f5-48c0-8a86-8f8e19b1191f" />

## RESULT
Thus the program for creating a database using ORM hass been executed successfully
