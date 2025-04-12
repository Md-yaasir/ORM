# Ex02 Django ORM Web Application
##REG-NO:212224040196
## Date:12-04-2025 

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![Uploading ER-DIAGRAM.jpg…]()




## DESIGN STEPS

### STEP 1:
Clone the problem from GitHub

### STEP 2:
Create a new app in Django project

### STEP 3:
Enter the code for admin.py and models.py

### STEP 4:
Execute Django admin and create details for 5 employee id

## PROGRAM
FOR MODELS:
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
FOR ADMIN:
```
from django.contrib import admin
from .models import Employee,EmployeeAdmin
admin.site.register(Employee,EmployeeAdmin)

```




## OUTPUT

![alt text](<Screenshot 2025-04-12 201342.png>)
![alt text](<Screenshot 2025-04-12 201809.png>)



## RESULT
Thus the program for creating a database using ORM hass been executed successfully
