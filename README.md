# Ex02 Django ORM Web Application.

### Date: 
### Name:Loshini.G
### Register Number:212223220051.
### Department: IT.

## AIM:
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM:
![Screenshot 2024-09-25 154040](https://github.com/user-attachments/assets/84d48dad-c7ca-4ab8-9397-21602c076fdc)



## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 7 clients

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

## OUTPUT:
![Screenshot 2024-09-25 155651](https://github.com/user-attachments/assets/c2904392-8932-49fc-86b5-e4883f68d9a4)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
