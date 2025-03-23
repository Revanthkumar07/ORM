# Ex02 Django ORM Web Application
# Date:23-03-2025
# AIM
To develop a Django application to store and retrieve data from a bank loan database using Object Relational Mapping(ORM).

# ENTITY RELATIONSHIP DIAGRAM
![image](https://github.com/user-attachments/assets/9b2a904f-68e3-4ade-951b-30f56ca0d628)

## DESIGN STEPS
## STEP 1:
Clone the problem from GitHub

## STEP 2:
Create a new app in Django project

## STEP 3:
Enter the code for admin.py and models.py

## STEP 4:
Execute Django admin and create details for 10 books

# PROGRAM
1. models.py
```
from django.db import models                                                                                                                      
from django.contrib import admin                                             
class book(models.Model):                    				      
   bookno=models.IntegerField(primary_key=True);                                                      
   authorname=models.CharField(max_length=50);                                                            
   price=models.IntegerField(help_text="enter price");                       
   qty=models.IntegerField();                                                
   bookname=models.CharField(max_length=50);                                 
class bookAdmin(admin.ModelAdmin):                                           
   list_display=("bookno","authorname","price","qty","bookname");
```
2. admin.py
```
from django.contrib import admin                                             
from .models import book,bookAdmin                                           
admin.site.register(book,bookAdmin)
```
# OUTPUT
Include the screenshot of your admin page.
![Screenshot 2025-03-23 205125](https://github.com/user-attachments/assets/e3e09e38-9e06-461c-8516-ee6c24c8c2dd)

![Screenshot 2025-03-23 205107](https://github.com/user-attachments/assets/9bf78503-1037-4203-96cb-6468a714962f)

# RESULT
Thus the program for creating a database using ORM hass been executed successfully
