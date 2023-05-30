# Django ORM Web Application

## AIM
To develop a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).

## Entity Relationship Diagram
![image](https://github.com/devesh-s1/django-orm-app/assets/121490523/86665b2a-61c8-471d-9b06-cd9f98ce004d)

Include your ER diagram here

## DESIGN STEPS

### STEP 1:
Fork and clone the repositary in to your IDE.
### STEP 2:
Create a django project and an app and a superuser account and run the server.

### STEP 3:
Modify changes in settings and write ur code on models and admin and run the server.

### STEP 4:
Login in to admin using your superuser account and populate the records.

## PROGRAM
```
from django.db import models
from django.contrib import admin

class Employee (models.Model):
   emp_id=models.CharField(primary_key=True,max_length=4,help_text='Employee ID')
   ename=models.CharField(max_length=50)
   post=models.CharField(max_length=20)
   phonenumber=models.IntegerField()
   salary=models.IntegerField()

class EmployeeAdmin(admin.ModelAdmin):
    list_display=('emp_id','ename','post','phonenumber','salary')
```

## OUTPUT
![image](https://github.com/devesh-s1/django-orm-app/assets/121490523/0d773ba4-d8a6-41a0-9820-7a3ee6359a8a)
Verifying Primary-Key
![image](https://github.com/devesh-s1/django-orm-app/assets/121490523/e9cfde0f-0012-4c3b-b54e-8ce064fc966a)

## RESULT
Thus we developed a Django application to store and retrieve data from a database using Object Relational Mapping(ORM).
