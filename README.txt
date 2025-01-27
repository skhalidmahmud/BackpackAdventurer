1. install python 3.x.x

> open any folder and run on cmd
>> python -m venv my_venv
>> my_venv\Scripts\activate
>> pip install Django
-> django-admin version || for check
3. 'pip freeze' for showing installed package
>> django-admin startproject AnyProjectName || for start new project

5. 'python manage.py runserver' for running the server
	'python manage.py runserver AnyPortNumber' like 5555 for change url port
6. 'python manage.py migrate' >> next to runserver **for viewing the table, use 'DB Browser for SQLite**
7. 'python manage.py createsuperuser' >> for use super user
8. for create views >> 
	create a folder as viwes.py
	write >
		from django.http import HttpResponse

			def home(request): ** any name**
				return HttpResponse("ANYTHING.")
	then open urls.py and call views
9. 
















>> 		{% extends "base.html" %}
		{% block content %}
		    <!-- start containt-->


		 	<!-- end containt-->
		{% endblock %}