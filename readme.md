(base) xxx@xxx-iMac % python3 -m venv djanog_env \
(base) xxx@xxx-iMac % cd djanog_env/bin \
(base) xxx@xxx-iMac bin % source activate


(djanog_env) (base) xxx@xxx-iMac bin % pip list
```
Package    Version
---------- -------
pip        22.0.4
setuptools 58.1.0
```

(djanog_env) (base) xxx@xxx-iMac bin % pip install django \
(djanog_env) (base) xxx@xxx-iMac bin % pip list \
Package    Version
---------- -------
asgiref    3.6.0
Django     4.1.7
pip        22.0.4
setuptools 58.1.0
sqlparse   0.4.3

(djanog_env) (base) xxx@xxx-iMac bi % python  \
Python 3.9.12 (main, Apr  5 2022, 01:53:17) \
[Clang 12.0.0 ] :: Anaconda, Inc. on darwin\
Type "help", "copyright", "credits" or "license" for more information.
```
>>> import django
>>> django.__version__
'4.1.7'
>>> exit()
```

create a file for django web, I put in ~ \
(djanog_env) (base) xxx@xxx-iMac ~ % cd django_web \
(djanog_env) (base) xxx@xxx-iMac django_web % django-admin startproject one\
(djanog_env) (base) xxx@xxx-iMac django_web % ls\
one\
(djanog_env) (base) xxx@xxx-iMac django_web % cd one\
(djanog_env) (base) xxx@xxx-iMac one % ls\
manage.py	one\
(djanog_env) (base) xxx@xxx-iMac one % cd one\
(djanog_env) (base) xxx@xxx-iMac one % ls\
__init__.py	asgi.py		settings.py	urls.py		wsgi.py\
(djanog_env) (base) xxx@xxx-iMac one % cd ..\
(djanog_env) (base) xxx@xxx-iMac one % ls\
manage.py	one\
(djanog_env) (base) xxx@xxx-iMac one % python manage.py startapp app\
(djanog_env) (base) xxx@xxx-iMac one % ls\
app		manage.py	one\
(djanog_env) (base) xxx@xxx-iMac one app % cd ..\
(djanog_env) (base) xxx@xxx-iMac one one % python manage.py runserver 0.0.0.0:8000 \
open your browser, and type localhost:8000\

![image]("https://user-images.githubusercontent.com/17458027/223188494-1d252599-73cc-4c5b-9b5b-0305d6d21ae1.png")

