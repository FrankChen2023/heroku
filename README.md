# heroku  
0. Set your environment  
    pip install flask  
    python version, virtual environment( python3 -m venv .venv)  
1. build connection with github (git clone...)  
1.5 pip install --upgrade pip  
2. pip install heroku  
3. curl https://cli-assets.heroku.com/install.sh | sh (install CLI tools)  
4. pip install gunicorn  
5. python3 -m pip freeze > requirements.txt  
6. create two file. (Procfile, runtime.txt)  
7. heroku login -i (build connection between our work and heroku)  
8. heroku create -a *application-name  
9. heroku git:remote -a story-generator-032022  
10. git add . -> git commit -m "*your words" -> git push heroku main  
