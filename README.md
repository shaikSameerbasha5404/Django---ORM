# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Creating a table using required detail in Django-ORM
### STEP 2:
Upload the python code
### STEP 3:
Push the code to github
## PROGRAM
```python
manage.py
from django.db import models
from django.contrib import admin


from django.contrib import admin
 Create your models here.
class Student(models.Model):
    referencenumber = models.CharField(max_length=10, help_text="Your Reference Number")
    name = models.CharField(max_length=100)
    age = models.IntegerField()
    email = models.EmailField()

class StudentAdmin(admin.ModelAdmin):
    list_display = ('referencenumber','name','age','email')


admin py

from .models import Student,StudentAdmin

admin.site.register(Student,StudentAdmin)    
```
## OUTPUT
![ORM_output](https://user-images.githubusercontent.com/118707756/213605379-5c4087b2-179f-4c62-8d97-e0144e7b08c2.png)
## RESULT
Thus the experiment executed successfully
