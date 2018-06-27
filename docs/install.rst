Install
=========

This is where you write how to get a new laptop to run this project.

Windows
"""""""""""""""""

| `git clone https://github.com/ebarras/cert_tracker.git`
| cd cert_tracker
| virtualenv.exe venv
| .\venv\Scripts\activate
| pip install -r .\requirements\local.txt
| createdb.exe -Upostgres (Get-Item -Path ".").Name
| createuser.exe -Upostgres $env:UserName
| python .\manage.py migrate
| python .\manage.py runserver 0.0.0.0:8000
