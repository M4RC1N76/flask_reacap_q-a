# Flask Recap with ANSWERS

This week we've built out the back end of an app and added data persistence in the form of PostgreSQL. This week we've been building the `M` in MVC.

![MVC](img/mvc.png)

Our next step will be to add Flask. Flask will provide us with the `V` and the `C`.

Let's review what Flask is and where it will fit in our applications.

Flask is a web framework for building web applications with Python. 

## Task
## ANSWERS:
Your task is to review the Events App that we built last week. Ask yourself the following questions:

1. What does the directory structure look like? 

The folder with Flask Homework contains directories with app/templates, controllers, models, static/CSS and templates. The directories mentioned above have different functions.


2. What are the different parts that make up the app?

The different parts of the application are:
    a) Modules - The Module Data Models. (__init__.py ( this file makes Python treat directories containing it as modules), Event class)
    b) Controllers (Views) - (__init__.py, )
    c) The applications in "app/init.py"
    d) The Templates (base and index, both HTML)
    e) Static/CSS



3. What are controllers responsible for?

The controllers are built from imports and routes. Imports are here to make sure that the correct functional links are made between models and users part views. the controllers contain @app.route('/') which are used to create 'routes' to forward the supported requests and any information encoded in request URLs.

4. What are templates responsible for?

Templates are responsible for storing static data and placeholders for dynamic data. Flask uses Jinja library to render templates. In our Flask homework we have index and base, both written in HTML. We will be able to use them, update them without need of writing them from the beginning every single time.

5. What is the static folder for?

Static folder contains CSS files, images, JavaScript files. Those files are called assets and are used by templates.

6. How do you think we will combine what we've done this week with Flask?

In My opinion we will combine everything we have learned so far. We know MVC working pattern and connecting blocks. We have learned about SQL language which is used to communicate with DataBase. we have also learned how to connect to database with psycopg2. The next step is to practice all we have learned and create full stack apps.   

7. How do you create a `route` in the controller?

We can create `route` by using the decorator in Flask. @app.route is used to bind URL to a function.
Route lays out all the order on a map and gives immediate access to their latest status changes.


8. The `models/events.py` file acted as some dummy data for our app. This will no longer be necessary. Why is that the case?

The `models/events.py` was created temporarily for the educational purpose. It was due to our lack of knowledge at that time about SQL language and proper DataBase. After introduction of SQL (which is most common language used to extract and organize data stored in a database) we will be able to connect to and use proper database.
