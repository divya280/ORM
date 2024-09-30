# Ex02 Django ORM Web Application
## Date: 30.09.2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM

![image](https://github.com/user-attachments/assets/3d15de26-0758-4384-8ff9-eeb115540284)



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

## admin.py:
```
from django.contrib import admin
from .models import bankloan,bankloanAdmin
admin.site.register(bankloan,bankloanAdmin)
```
## models.py:
```
from django.db import models
from django.contrib import admin
class bankloan (models.Model):
    name=models.CharField(max_length=100)
    account_number =models.IntegerField(primary_key=True)
    loan_amount=models.IntegerField()
    loan_limit=models.IntegerField()
    contact_number=models.IntegerField()
    email=models.EmailField()
 
class bankloanAdmin(admin.ModelAdmin):
    list_display=('name','account_number','loan_amount','loan_limit','contact_number','email')
```

## OUTPUT

![image](https://github.com/user-attachments/assets/b0f86b40-6181-4d09-8fa8-446847eea271)


## RESULT
Thus the program for creating a database using ORM hass been executed successfully
