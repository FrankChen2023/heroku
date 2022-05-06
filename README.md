# heroku  
0. Set your environment  
    (command.) pip install flask  
    python version, virtual environment  
        (command.) python3 -m venv .venv  
        (command.) source .venv/bin/activate  
1. build connection with github  
    (command.)git clone + SSH key  
1.5 (command.) pip install --upgrade pip  
2. (command.) pip install heroku  
3. (command.) curl https://cli-assets.heroku.com/install.sh | sh (install CLI tools)  
4. (command.) pip install gunicorn  
5. (command.) python3 -m pip freeze > requirements.txt  
    Delete all contents but heroku, gunicorn, django.  
6. create two file. (Procfile, runtime.txt)  
    Procfile: web: gunicorn mysite.wsgi --log-file -  
    runtime.txt: python-3.7.0 (or 3.9.0)  
7. (command.) heroku login -i (build connection between our work and heroku)  
8. (command.) heroku create -a *application-name (eg, heroku create -a myapp-01012202)  
9. (command.) heroku git:remote -a *application-name (eg, heroku git:remote -a myapp-01012202)    
10. git add . -> git commit -m "*your words" -> git push heroku main  
