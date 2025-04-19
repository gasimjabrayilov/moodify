
💡 Project Setup Guide
📁 Repository Initialization

    Created an empty GitHub repository and cloned it locally.

    Added requirements.txt (for Django dependencies) and README.md.

🐍 Virtual Environment

    Created a virtual environment:

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