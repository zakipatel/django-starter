# django-starter

## Set Up 

https://docs.djangoproject.com/en/3.0/topics/install/#installing-official-release

1. Install homebrew https://brew.sh/

` echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> /Users/zaki/.zprofile`
`zaki@zakis-MacBook-Pro ~ % eval "$(/opt/homebrew/bin/brew shellenv)"`

2. Install pyenv and python
- (https://opensource.com/article/19/5/python-3-default-mac) 
- https://github.com/pyenv/pyenv#installation
- https://laict.medium.com/install-python-on-macos-11-m1-apple-silicon-using-pyenv-12e0729427a9

`brew install pyenv`

`xcode-select --install`

`brew install openssl readline sqlite3 xz zlib`

`pyenv install 3.7.3`
`pyenv install 3.9.4`

` pyenv global 3.9.4`
` pyenv version`

3. Install pip 
- https://docs.python.org/3/tutorial/venv.html

`python3 -m venv tutorial-env`

`source tutorial-env/bin/activate`

`pip -version` 


4. Install django 

`python -m pip install Django`

Verify  
- `venv > python`
- `import django`
- `print(django.get_version())`

or `python -m django --version`


5. create a django project 

`python manage.py startapp polls`
  
7. run the server 
`$ python manage.py runserver`
`http://127.0.0.1:8000/`

8. Wire up the index view 
9. Add app to install 
11. Write models
12.  run migrations
13.  python manage.py shell
14.  python manage.py createsuperuser

 http://127.0.0.1:8000/admin/.
 
 
 sudo lsof -t -i tcp:8000 | xargs kill -9
