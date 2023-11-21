# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## DESIGN STEPS

### STEP 1:
Clone the problem into Github
### STEP 2:
Create a new app in Django project
### STEP 3:
Enter the code for admin.py and model.py
### STEP 4:
Make Migration and push into Respirority
## PROGRAM
```
admin.py
from django.contrib import admin
from .models import Student,StudentAdmin

# Register your models here.
admin.site.register(Student,StudentAdmin)

model.py
from django.db import models
from django.contrib import admin

# Create your models here.
class Student (models.Model):
    referencenumber=models.CharField(max_length=20,help_text="reference number")
    name=models.CharField(max_length=100)
    age=models.IntegerField()
    email=models.EmailField()

class StudentAdmin(admin.ModelAdmin):
    list_display=('referencenumber','name','age','email')

```

## OUTPUT
![output](./orm.png)

## RESULT
Thus the program for creating a database using ORM has been Executed  successfully.