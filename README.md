# Ex02 Time Table
# Date:7/02/2026
# AIM
To write a html webpage page to display your slot timetable.

# ALGORITHM
## STEP 1
Create a Django-admin Interface.

## STEP 2
Create a static folder and inert HTML code.

## STEP 3
Create a simple table using `<table>` tag in html.

## STEP 4
Add header row using `<th>` tag.

## STEP 5
Add your timetable using `<td>` tag.

## STEP 6
Execute the program using runserver command.

# PROGRAM

timetable.html
```
{% load static %}

<!DOCTYPE html>

<html>
    <head>
        <title>SLOT TIMETABLE</title>

        <link rel="stylesheet" href="{% static 'CSS.css' %}">

        <link rel="icon" href="{% static 'SEC-Logo-1.png'%}">

    </head>

    <body>
        <center>
            <img src = "{% static 'SAVEETHA.png' %}" height="100" width="700">
        </center>    
        <h2>SLOT TIMETABLE</h2>
        <h3> vaishnavi v- 25012347</h3>
        <center>
        <table>
        <tr>
            <th> DAY/TIME</th>
            <th> MONDAY</th>
            <th> TUESDAY</th>
            <th> WEDNESDAY</th>
            <th> THURSDAY</th>
            <th> FRIDAY</th>
            <th> SATURDAY</th>
        </tr>
        <tr>
            <th>8-10</th>
            <td colspan="3">WEB</td>
            <td rowspan="2">FREE SLOT</td>
            <td>FREE SLOT</td>
            <td>PYTHON</td>
         </tr>
         <tr>
            <th> 10-12</th>
            <td> ENG</td>
            <td> PYTHON</td>
            <td>FREE SLOT</td>
            <td colspan="2">ENG</td>
        </tr>
        <tr>
            <th> 12-1</th>
            <td colspan="6"><b>LUNCH BREAK </b> </td>
        </tr>
        <tr>
            <th> 1-3</th> 
            <td> WEB</td>
            <td> FREE SLOT</td>
            <td> MENTOR MEET</td>
            <td> FREE SLOT</td>
             <td> WEB</td>
             <td> ENG</td>
            </tr>
            <tr>
                <th>3-5</th>
                <td> FREE SLOT</td> 
                <td colspan="3"> PYTHON</td>
                <td colspan="2">FREE SLOT</td>
            </tr>
        </table>
        <table>
            <tr background-color:rgb(255, 145, 217);>
                <th> S.NO</th>
                <th> SUBJECT CODE</th>
                <th> SUBJECT NAME</th>
            </tr>
            <tr>
                <th background-color:rgb(237, 190, 221);>1</th>
                <td> 19AI414</td>
                <td> Fundamentals of Web Application Development</td>
            </tr>
            <tr>
                <th background-color:rgb(237, 190, 221);>2</th>
                <td> 19AI301</td>
                <td>Python Programming</td>
            </tr>
            <tr>
                <th background-color:rgb(237, 190, 221);>3</th>
                <td>19EN101</td>
                <td>Communicative English</td>
            </tr>
        </table>
    </center>
</body> 
</html>
```

CSS.css
```

            table{
                background-color:rgb(127, 180, 244);
                border:2px solid black;
                width:50%;
                text-align:center;
                border-collapse:collapse;
                padding:10px;
            }
            th{
                border: 2px solid black;
                text-align:center;
                padding:10px;
                font-family:"Footlight MT Light";
            }
            td{
                text-align:center;
                padding:10px;
                border:2px solid black;
                background-color:rgb(206, 231, 252);
                font-family: "Palatino Linotype";
            }
            h3{
                text-align:center;
                font-family: "Lucida Calligraphy";
            }
            h2{
                text-align: center;
                font-family:"Eras Medium ITC" ;
            }
            body {
                 font-family: "Montserrat Bold";
                 background-color: rgb(215, 234, 255);
            }
```
views.py
```
from django.shortcuts import render

def home(request):
    return render(request, 'timetable.html')
```
urls.py
```
from django.contrib import admin
from django.urls import path
from slot_app import views

urlpatterns = [
    path('admin/', admin.site.urls),
    path('', views.home)
    
]
```
# OUTPUT:

<img width="1907" height="1086" alt="image" src="https://github.com/user-attachments/assets/60f5ab22-094f-4d64-9ff0-29cd669ca115" />

# RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
