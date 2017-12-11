# Server for connectiv building automation

This built with django, to start the dev server use `python manage.py runserver`

To bootstrap:  
pip install -r requirements.txt  
define database creds (or change to sqllite) in settings.py  
update your secret key in secrets.py  
python manage.py migrate  
python manage.py createsuperuser  

  
http://localhost:8000  
login with what you created in createsuperuser  


