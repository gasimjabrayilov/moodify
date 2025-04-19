
💡 Project Setup Guide
📁 Repository Initialization

    Created an empty GitHub repository and cloned it locally.

    Added requirements.txt (for Django dependencies) and README.md.

🐍 Virtual Environment Created a virtual environment:

    python3 -m venv myenv
    source myenv/bin/activate



Added myenv/ to .gitignore to exclude it from version control.

⚙️ Django Setup
Created a new Django project:

    django-admin startproject devsearch

Created a new app:


    python3 manage.py startapp projects

Registered the new app by adding it to INSTALLED_APPS in devsearch/settings.py:
    'projects.apps.ProjectsConfig',



🚀 Local Server Test
Verified everything works by running the development server:

    python3 manage.py runserver



In the projects app I created urls.py for storing
Last thing for connecting projects file as a url on django we need on urls.py 
    from django.urls import path, and also add "include"

also in urlpatterns > path('', include('projects.urls'))



I created templates and added projects.html file 
then we need to go to main settings.py and 
 1. import os
 2. >TEMPLATES>"DIRS">os.path.join(BASE_DIR, 'templates'),
then I moded to views.py and added : return render(request, 'projects.html')


When you want to create new html page adding just new  view and url is enough*


Inside of projects I created templates/projects and I moved project.html and projects.html files inside of it
