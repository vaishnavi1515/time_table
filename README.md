# Ex03 Time Table
# Date:21/10/2024
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

# PROGRAM:
~~~
<!DOCTYPE html>
<html>
<head>
    <title>Time Table - Vaishnavi V</title>
    <style>
        table {
            width: 100%;
            border-collapse: collapse;
        }
        th, td {
            border: 1px solid black;
            text-align: center;
            padding: 10px;
        }
        th {
            background-color: #ffd700; /* Yellow */
        }
        td {
            background-color: #87CEEB; /* Sky blue */
        }
        h1, h2 {
            text-align: center;
        }
        .header {
            display: flex;
            justify-content: space-between;
        }
    </style>
</head>
<body>
    <h2>SLOT TIME TABLE - VAISHNAVI V (24900560)</h2>

    <table>
        <tr>
            <th>Day/Time</th>
            <th>Monday</th>
            <th>Tuesday</th>
            <th>Wednesday</th>
            <th>Thursday</th>
            <th>Friday</th>
            <th>Saturday</th>
        </tr>
        <tr>
            <th>8-10</th>
            <td>Free slot</td>
            <td>Chemistry</td>
            <td>Free slot</td>
            <td>Machine learning</td>
            <td>Statistics</td>
            <td>Statistics</td>
        </tr>
        <tr>
            <th>10-12</th>
            <td>Career Development</td>
            <td>Statistics</td>
            <td>Free slot</td>
            <td>C programming</td>
            <td>Web application</td>
            <td>Web application</td>
        </tr>
        <tr>
            <th>12-1</th>
            <td colspan="6">Lunch</td>
        </tr>
        <tr>
            <th>1-3</th>
            <td>Web application</td>
            <td>C programming</td>
            <td>Mentor meet</td>
            <td>Chemistry</td>
            <td>Human values</td>
            <td>Free slot</td>
        </tr>
    </table>

    <h2>Subject Codes</h2>
    <table>
        <tr>
            <th>S.No.</th>
            <th>Subject Code</th>
            <th>Subject Name</th>
        </tr>
        <tr>
            <td>1</td>
            <td>19EY708</td>
            <td>Career Development</td>
        </tr>
        <tr>
            <td>2</td>
            <td>19AI404</td>
            <td>Web application</td>
        </tr>
        <tr>
            <td>3</td>
            <td>19CY205</td>
            <td>Chemistry</td>
        </tr>
        <tr>
            <td>4</td>
            <td>19MA211</td>
            <td>Statistics</td>
        </tr>
        <tr>
            <td>5</td>
            <td>19AI304</td>
            <td>C programming</td>
        </tr>
        <tr>
            <td>6</td>
            <td>19AI410</td>
            <td>Machine learning</td>
        </tr>
        <tr>
            <td>7</td>
            <td>SH7801</td>
            <td>Human values</td>
        </tr>
    </table>
</body>
</html>
~~~
# OUTPUT:

![image](https://github.com/user-attachments/assets/ae539acf-f394-458f-9880-2bc269f12784)

# RESULT
The program for creating slot timetable using basic HTML tags is executed successfully.
