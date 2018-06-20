Install
=========

This is where you write how to get a new laptop to run this project.

## Windows DEV Environment
git clone https://github.com/ebarras/cert_tracker.git
cd cert_tracker
virtualenv venv
set-executionpolicy RemoteSigned
venv\Scripts\activate
pip install -r requirements/local.txt
createdb.exe cert_tracker
# To Fix User Issue
createuser.exe -Upostgres <username>
python manage.py runserver 0.0.0.0:8000