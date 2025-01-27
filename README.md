# How to install and create Django?

#### 1. install python 3.x.x `Make sure to check Path`

> Then open any folder and run on cmd

#### 2. Create **env**
```cmd
python-m venv env
```
#### 3. Activate scripts
```cmd
my_venv\Scripts\activate
```

#### 4. Install Django
```cmd
pip install Django
```

> If you need to show install is procedure or not :
> ```cmd
> django-admin version
> ```
> ```cmd
> pip freeze
> ```

#### 5. Start Django New Project
```cmd
django-admin startproject `AnyProjectName`
```

#### 6. Run runserver
```cmd
python manage.py runserver
```
> `python manage.py runserver AnyPortNumber` like 5555 for change url port

#### 7. Migrate and Createsuperuser
> next to runserver **for viewing the table, use 'DB Browser for SQLite**
```cmd
python manage.py migrate
```
> for use super user
```cmd
python manage.py createsuperuser
```

#### 8. Create views on Project:

> for create views
> create a new py file as viwes.py on project directory
> And modify as
```python
from django.http import HttpResponse
from django.shortcuts import render

def `AnyName`(request):
    return render(request, "`index.html`")
def `test`(request):
    return HttpResponse("`This is home on <b>Test<b> page.`")
```
> then open urls.py and call views

#### 9. 

```python
>> 		{% extends "base.html" %}
		{% block content %}
		    <!-- start containt-->


		 	

<!-- end containt-->
		{% endblock %}
```