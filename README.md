# Ex02 Django ORM Web Application
##REG-NO:212224040196
## Date:12-04-2025 

## AIM
To develop a Django application to store and retrieve data from Movies Database using Object Relational Mapping(ORM).

## ENTITY RELATIONSHIP DIAGRAM
![Screenshot 2025-04-17 110407](https://github.com/user-attachments/assets/0c0fa11c-e26b-4a9a-ad4c-30cc3aa9ce1e)



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
FOR MODELS:
```
from django.db import models
from django.contrib import admin
class Movie(models.Model):
    mid=models.IntegerField()
    name=models.CharField(max_length=100)
    mail=models.EmailField(max_length=100)
    mname=models.CharField(max_length=100)
    phone=models.IntegerField()
    datetime=models.DateTimeField()
    seats=models.IntegerField()
class MovieAdmin(admin.ModelAdmin):
    list_display=('mid','name','mail','mname','phone','datetime','seats')


```
FOR ADMIN:
```
from django.contrib import admin
from .models import Movie,MovieAdmin
admin.site.register(Movie,MovieAdmin)

```




## OUTPUT

![Screenshot 2025-04-17 100243](https://github.com/user-attachments/assets/57be7e61-f0ad-4e3f-838a-2742a7f83392)
![Screenshot 2025-04-17 100221](https://github.com/user-attachments/assets/ea20d7cf-c779-438d-b301-2f657d08cf9c)




## RESULT
Thus the program for creating a database using ORM hass been executed successfully
