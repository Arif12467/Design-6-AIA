# Lab 4 [WIP]
## Labs 4A and 4B: Django and Django REST

### Install Django and Django REST framework on Raspberry Pi
```ssh
$ pip3 -V
$ pip3 list
$ sudo pip3 install -U setuptools
$ sudo pip3 install -U django
$ sudo pip3 install -U djangorestframework
$ sudo pip3 install -U django-filter
$ sudo pip3 install -U markdown
$ sudo pip3 install -U requests
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/651ee6043b2a7871bf19cec2da4a24fef0f8ce3d/Lab%204/Photos/pip3_-V-list.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/651ee6043b2a7871bf19cec2da4a24fef0f8ce3d/Lab%204/Photos/pip3_-V-list_continued.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/651ee6043b2a7871bf19cec2da4a24fef0f8ce3d/Lab%204/Photos/sudo_pip3_-U_setuptools-django-filter.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/47ae546ceabbf7e9b8fda34f5d4026d87dab7f46/Lab%204/Photos/sudo_pip3_install_-U_markdown-requests.png)


### Install MariaDB server and client on Raspberry Pi
```ssh
$ sudo apt update
$ sudo apt install mariadb-server mariadb-client
$ sudo apt install python3-mysqldb
$ sudo pip3 install -U mysqlclient
$ sudo mysql_secure_installation
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d842a7165293857541e7c7fb859840987d431f01/Lab%204/Photos/sudo_apt_update.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/cb1d7a86950e0f5a27f128888d5405a0a1e9af08/Lab%204/Photos/sudo_apt_install_mariadb-server_mariadb-client.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/cb1d7a86950e0f5a27f128888d5405a0a1e9af08/Lab%204/Photos/sudo_apt_install_mariadb-server_mariadb-client-1.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/cb1d7a86950e0f5a27f128888d5405a0a1e9af08/Lab%204/Photos/sudo_apt_install_mariadb-server_mariadb-client-2.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/b5a66b2989805dad38a2f8f24e49f358d0f9c814/Lab%204/Photos/sudo_apt_install_python3-mysqldb.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/82ccccf333503f61607f45b93d344554ce15e27d/Lab%204/Photos/sudo_pip3_install_-U_mysqlclient.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/82ccccf333503f61607f45b93d344554ce15e27d/Lab%204/Photos/sudo_mysql_secure_installation.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/82ccccf333503f61607f45b93d344554ce15e27d/Lab%204/Photos/sudo_mysql_secure_installation-2.png)


### Django Project "Stevens"
```ssh
$ django-admin startproject stevens
$ cd stevens
$ ls
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d3d2e8bea70164a56152c9e280e9b1c485ae0c1e/Lab%204/Photos/django-admin-ls.png)


```ssh
$ python3 manage.py startapp myapp
$ ls
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/269a51cbe71a742c65db173e0a1919af3039cad6/Lab%204/Photos/python3_managepy_startapp.png)


```ssh
$ sudo mysql -u root -p
Enter password: PASSWORD
MariaDB [(none)]> use mysql
MariaDB [mysql]> select user, host from mysql.user;
MariaDB [mysql]> create user pi@localhost identified by 'PASSWORD';
MariaDB [mysql]> show databases;
MariaDB [mysql]> create database stevens;
MariaDB [mysql]> grant all privileges on stevens.* to pi@localhost;
MariaDB [mysql]> quit
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/269a51cbe71a742c65db173e0a1919af3039cad6/Lab%204/Photos/sudo_mysql_-u_root_-p-create_user.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/269a51cbe71a742c65db173e0a1919af3039cad6/Lab%204/Photos/sudo_mysql_-u_root_-p.png)


```ssh
$ cd stevens
$ ls
$ nano settings.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/269a51cbe71a742c65db173e0a1919af3039cad6/Lab%204/Photos/settingspy-nano.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/269a51cbe71a742c65db173e0a1919af3039cad6/Lab%204/Photos/settingspy.png)


```ssh
$ cp ~/iot/lesson4/stevens/urls.py .
$ cd ..
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/21bde8b1b3512f228bf45373f2471c03110de6e4/Lab%204/Photos/copy%20urls.py.png)


```ssh
$ cd myapp
$ ls
$ cp ~/iot/lesson4/stevens/admin.py .
$ cp ~/iot/lesson4/stevens/models.py .
$ cp ~/iot/lesson4/stevens/views.py .
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/21bde8b1b3512f228bf45373f2471c03110de6e4/Lab%204/Photos/copy%20adminpy.png)


```ssh
$ mkdir static templates
$ cd templates
$ mkdir myapp
$ cd myapp
$ cp ~/iot/lesson4/stevens/index.html .
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/21bde8b1b3512f228bf45373f2471c03110de6e4/Lab%204/Photos/copy_indexhtml.png)


```ssh
$ nano index.html
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/1587782f85f5ed5cf2028f5843b202167e814186/Lab%204/Photos/nano%20indexhtml.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/1587782f85f5ed5cf2028f5843b202167e814186/Lab%204/Photos/API_key.png)


```ssh
$ cd ~/stevens/myapp/static
$ cp ~/iot/lesson4/static/favicon.ico .
$ mkdir myapp
$ cd myapp
$ cp ~/iot/lesson4/static/*css .
$ cp ~/iot/lesson4/static/*js .
$ cd ~/stevens
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/c4e3f80c905e25410d3f8847eb610db5eec73e8e/Lab%204/Photos/Copy_static_files.png)


```ssh
$ python3 manage.py makemigrations myapp
$ python3 manage.py migrate
$ python3 manage.py createsuperuser
Username (leave blank to use 'pi'):
Email address: aamzad@stevens.edu
Password: 
Password (again): 
Superuser created successfully.
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/c4e3f80c905e25410d3f8847eb610db5eec73e8e/Lab%204/Photos/python3_managpy_stevens.png)


```ssh
$ python3 manage.py runserver
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/c4e3f80c905e25410d3f8847eb610db5eec73e8e/Lab%204/Photos/python3_manage.py_runserver.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/c4e3f80c905e25410d3f8847eb610db5eec73e8e/Lab%204/Photos/Running_server.png)


```ssh
$ python3 manage.py runserver 0.0.0.0:8000
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/c4e3f80c905e25410d3f8847eb610db5eec73e8e/Lab%204/Photos/1.png)


### Django REST Project "MyCPU"
```ssh
$ django-admin startproject mycpu
$ cd mycpu
$ ls
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/c784c653c60c4066b29d63a93ed1bc48f5f644a0/Lab%204/Photos/django-admin_startproject_mycpu.png)


```ssh
$ python3 manage.py startapp myapp
$ ls
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/c784c653c60c4066b29d63a93ed1bc48f5f644a0/Lab%204/Photos/start_a_django_app.png)


```ssh
$ cd mycpu
$ ls
$ nano settings.py
$ cp ~/iot/lesson4/mycpu/urls.py .
$ cd ..
$ cd myapp
$ ls
$ cp ~/iot/lesson4/mycpu/admin.py .
$ cp ~/iot/lesson4/mycpu/models.py .
$ cp ~/iot/lesson4/mycpu/views.py .
$ cp ~/iot/lesson4/mycpu/serializers.py .
$ nano views.py
$ mkdir static templates
$ cd templates
$ mkdir myapp
$ cd myapp
$ cp ~/iot/lesson4/mycpu/index.html .
$ nano index.html
$ cd ~/mycpu/myapp/static
$ cp ~/iot/lesson4/static/favicon.ico .
$ mkdir myapp
$ cd myapp
$ cp ~/iot/lesson4/static/*css .
$ cp ~/iot/lesson4/static/*js .
$ cd ~/mycpu
$ ls
$ cp ~/iot/lesson4/mycpu/controller.py .
$ nano controller.py
$ sudo pip install -U psutil
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/c784c653c60c4066b29d63a93ed1bc48f5f644a0/Lab%204/Photos/cd_mycpu-sudo_pip_install_-U_psutil.png)


```ssh
$ python3 manage.py makemigrations myapp
$ python3 manage.py migrate
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/026e0e8f587df76fbef72d034cb8ef8326d04223/Lab%204/Photos/python_managepy.png)


```ssh
$ python3 manage.py createsuperuser
Username (leave blank to use '_'): admin
Email address: aamzad@stevens.edu
Password: 
Password (again): 
The password is too similar to the username.
This password is too short. It must contain at least 8 characters.
This password is too common.
Bypass password validation and create user anyway? [y/N]: y
Superuser created successfully.

$ python3 manage.py runserver
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/026e0e8f587df76fbef72d034cb8ef8326d04223/Lab%204/Photos/python3-runserver.png)


**Dt List**
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/026e0e8f587df76fbef72d034cb8ef8326d04223/Lab%204/Photos/Dt_list.png)

**Cpu List**
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/026e0e8f587df76fbef72d034cb8ef8326d04223/Lab%204/Photos/Cpu_list.png)

**Mem List**
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/026e0e8f587df76fbef72d034cb8ef8326d04223/Lab%204/Photos/Mem_list.png)


```ssh
$ python controller.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/7a8363fc9dc25f51673dc9ee7749cf5fde3be7a6/Lab%204/Photos/running_server_mycpu.png)

```ssh
$ python manage.py runserver 0.0.0.0:8000
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/7a8363fc9dc25f51673dc9ee7749cf5fde3be7a6/Lab%204/Photos/2.png)


## Lab 4C: Flask

### Run Flask server 
```ssh
$ cd ~/iot/lesson4
python3 hello_world.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/317bba924c2cafd687e7bc682597e0a5b3d6f754/Lab%204/Photos/cd%20helloworld.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/317bba924c2cafd687e7bc682597e0a5b3d6f754/Lab%204/Photos/Lab%204C%20-1.png)


### Install Flask-Ask and Ngrok for Alexa Skill Kit (ASK)
```ssh
$ sudo pip3 install -U flask-ask
$ sudo pip3 install 'cryptography<2.2'
$ sudo wget https://bin.equinox.io/c/4VmDzA7iaHb/ngrok-stable-linux-arm.zip
$ sudo unzip ngrok-stable-linux-arm.zip
$ ./ngrok http 5000
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4c0c8d9ba1aa7049e9618b6c6d17c9febbbbae09/Lab%204/Photos/install_flask-ask.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4c0c8d9ba1aa7049e9618b6c6d17c9febbbbae09/Lab%204/Photos/install_cryptography.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4c0c8d9ba1aa7049e9618b6c6d17c9febbbbae09/Lab%204/Photos/ngork%20install.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4c0c8d9ba1aa7049e9618b6c6d17c9febbbbae09/Lab%204/Photos/ngrok.png)


### Memory Game
```ssh
$ cd ~/iot/lesson4
$ python3 memory_game.py
```
![This is an image]()


### Open a browser and sign in Alexa Developer Console
![This is an image]()
Note: Alexa Developer was broken


