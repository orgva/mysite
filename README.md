"mysite" 
Following the Sources:
https://www.javatpoint.com/django-deploy-on-github
&
https://djangocentral.com/building-a-blog-application-with-django/

In case of deployment to pythonanywhere ->
Please follow:
https://help.pythonanywhere.com/pages/DeployExistingDjangoProject/

Pay attention to your python version in order to create a virtualenv. 
In my case I used python3.8

Instead of ./manage.py migrate (database setup, bash) use:
python ./manage.py migrate

In case of INVALID HTTP_HOST header, go to mysite/mysite/settings and add to allowed_hosts ['myusername.pythonanywhere.com'] 

In case of python manage.py startapp blog:
use django-admin startapp blog

How to activate the venv in pythonanywhere:
workon mysite-virtualenv
