# Ex02 Django ORM Web Application
## Date: 14-11-2024

## AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![ER DIAGRAM WEB](https://github.com/user-attachments/assets/6bc68eb7-8ad5-4be4-a49f-5c7a68f2cf0e)



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
from django.contrib import admin
from.models import Bank,BankAdmin
admin.site.register(Bank,BankAdmin)

from django.db import models
from django.contrib import admin
class Bank(models.Model):
  Name=models.CharField(max_length=10)
  Accountno=models.IntegerField(primary_key="accountno")
  Aadharno=models.IntegerField()
  DoB=models.DateField()
  Email=models.EmailField()
  Branch=models.CharField(max_length=21)

class BankAdmin(admin.ModelAdmin):
  list_display=('Name','Accountno','Aadharno','DoB','Email','Branch')

```


## OUTPUT

![Screenshot (9)](https://github.com/user-attachments/assets/f63f4b59-dcf4-4f07-ae7e-2311c4828b0f)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
