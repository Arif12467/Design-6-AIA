# Lab 3
## Python

```ssh
$ sudo apt update
$ sudo apt install python3-pip
$ pip3 list
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/79fb1de537663dfe2650c688e8bd0efa9f82681f/Lab%203/Photos/sudo-pip3.png)

```ssh
$ sudo pip3 install -U jdcal astral geopy
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d17252f981a6d98475089ca772ffc6d515d80525/Lab%203/Photos/pip%20install.png)

```ssh
$ cd iot
$ git pull
$ cd lesson3
$ python3 julian.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/cd-julian.png)

```ssh
$ python3 date_example.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/date_example.png)

```ssh
$ python3 datetime_example.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/datetime_example.png)

```ssh
$ python3 time_example.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/time_example.png)

```ssh
$ python3 sun.py 'New York'
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/sun.png)

```ssh
$ python3 moon.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/moon.png)

```ssh
$ python3 coordinates.py 'SC Williams Library'
$ python3 address.py '40.74480675, -74.02532862031404'
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/coordinates-address.png)

```ssh
$ python3 cpu.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/cpu.png)

```ssh
$ python3 battery.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/battery.png)

```ssh
$ python3 documentstats.py document.txt
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/05b8306d740f2f42fe6496d4c8d48a4f8f93753e/Lab%203/Photos/documentstats.png)

```ssh
$ python3 system_info.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/6494d0b0be218b14470b264f4b8ecc8efc10701b/Lab%203/Photos/system_info.png)



## Lab 3E: PyPy

```ssh
$ cd ~/iot/lesson3/pypy
$ gcc -o test test.c
$ time ./test
$ time pypy test.py
$ time python test.py
$ time python3 test.py
$ pypy -m cProfile test.py
$ python -m cProfile test.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/6494d0b0be218b14470b264f4b8ecc8efc10701b/Lab%203/Photos/cd-python_-m.png)

```ssh
$ python3 -m cProfile test.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/6494d0b0be218b14470b264f4b8ecc8efc10701b/Lab%203/Photos/python3_-m.png)



## Lab 3F: Doxygen

```ssh
$ sudo apt install doxygen html2text
$ cd ~/demo
$ cp ~/iot/lesson3/pyexample.py .
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/6494d0b0be218b14470b264f4b8ecc8efc10701b/Lab%203/Photos/sudo-cp.png)

```ssh
$ doxygen -g doxygen.config
$ nano doxygen.config
$ doxygen doxygen.config
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/6494d0b0be218b14470b264f4b8ecc8efc10701b/Lab%203/Photos/doxyegn-doxygen.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/6494d0b0be218b14470b264f4b8ecc8efc10701b/Lab%203/Photos/doxygen_continued.png)

```ssh
$ cd html
$ html2text annotated.html
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/6494d0b0be218b14470b264f4b8ecc8efc10701b/Lab%203/Photos/cd-html2text.png)
