# Server for connectiv building automation

This built with django, to start the dev server use `python manage.py runserver`   
Or, python3 if you run multiple environments. Either way, you should *not* be running this on python 2.x  
  

To bootstrap:  
git clone this repo    
install pipenv - http://docs.python-guide.org/en/latest/dev/virtualenvs/  
(pipenv has replaced requirements.txt)  
  
change manage.py dataServer.local_settings to your settings file (in dataServer/settings.py for example) 
define database creds (or change to sqllite) in settings.py 
update your secret key in secrets.py  

*this migrate will create your DB schema in the target DB*  
python manage.py migrate   
  
python manage.py createsuperuser  

  
visit:  
http://localhost:8000  
login with what you created in createsuperuser  



to grab data use
`curl -H 'Accept: application/json; indent=4' -u admin:testpw http://138.197.216.233:8000/networkconnectivity/networkData/`

