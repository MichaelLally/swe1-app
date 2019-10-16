# swe1-app
[![Build Status](https://travis-ci.com/MichaelLally/swe1-app.svg?branch=master)](https://travis-ci.com/MichaelLally/swe1-app)
[![Coverage Status](https://coveralls.io/repos/github/MichaelLally/swe1-app/badge.svg?branch=master)](https://coveralls.io/github/MichaelLally/swe1-app?branch=master)
CS-GY 6063 Software Engineering Django App

### Requirements
gunicorn
django-heroku

### MacOS (Mojave)
brew install postgresql
sudo installer -pkg /Library/Developer/CommandLineTools/Packages/ macOS_SDK_headers_for_macOS_10.14.pkg -target /
pip3 install django-heroku --user

heroku run python manage.py migrate
heroku run python manage.py makemigrations polls
heroku run python manage.py sqlmigrate polls 0001
heroku run python manage.py migrate