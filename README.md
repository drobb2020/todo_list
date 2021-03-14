# Python Django To Do App

<img align="left" alt="Python" width=75px src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/python/python.png" />
<img align="left" alt="Flask" width=75px src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/django/django.png" />

This is a Django application based on a [YouTube Video](https://www.youtube.com/watch?v=llbtoQTt4qw&t=3284s) presented by Dennis Ivy. Please check out his channel on [YouTube](https://www.youtube.com/channel/UCTZRcDjjkVajGL6wd76UnGg). Also, you should take the time to read this [article](https://www.dennisivy.com/post/django-class-based-views/) on class based views in django. The article has many great links to django resources.

This was a quick and fun django project and taught me a lot about class based views in django.

## Starting the To Do Project

1. Create a virtual environment with the command:

    ``` python
    python3 -m venv todo_env 
    ```

2. Create a directory named todo_list.

3. Start the virtual environment created in #1 using the command:
   - Mac

   ``` python
   source todo_env/bin/activate
   ```

   - Windows

   ``` python
   todo_env\Scripts\activate.bat
    ```

4. Use pip to install the Django module:

    ``` python
    pip install django 
    ```  

5. Run django-admin to start the project with the command:

    ``` python
    django-admin startproject todo_list 
    ```

6. CD into the todo_list directory. You should see a manage.py file in the folder. You can run the following command to start the server:

    ``` python
    python manage.py runserver 
    ```

7. You should get a message like this:

    Django version 3.1.7, using settings 'Django_Project.settings'
    Starting development server at [http://127.0.0.1:8000/](http://127.0.0.1:8000)
    Quit the server with CONTROL-C.

8. You can launch a web browser and go to the above URL and you should see a default django landing page.

## Starting a Django Application

Once the server is functional you can then start your application. For this project the command used is:

``` python
python manage.py startapp base
```

This will create a new folder named base in the django_project directory and populate it with the necessary files to start coding your application.

## Migrations

To access the Admin page feature of Django you have to run the initial migration to initialize the auth user database. The commands used are:

``` python
python manage.py makemigrations 
```

``` python
python manage.py migrate 
```

``` python
python manage.py createsuperuser 
```

When you run createsuperuser you will be prompted to enter a username and password for the default admin user. You can then run the server and login to the admin page at [http://127.0.0.1:8000/admin](http://127.0.0.1:8000/admin).
