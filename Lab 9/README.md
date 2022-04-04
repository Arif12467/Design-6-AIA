# Lab 9
## Lab 9A: YANG

```ssh
$ sudo apt install libxml2-dev libxslt1-dev
$ sudo pip3 install -U lxml pyang
$ cp ~/iot/lesson9/intrusiondetection.yang ~/demo
$ cd ~/demo
$ cat intrusiondetection.yang
$ pyang -f yin -o intrusiondetection.yin intrusiondetection.yang
$ cat intrusiondetection.yin
$ pyang -f uml -o intrusiondetection.uml intrusiondetection.yang --uml-no=stereotypes,annotation,typedef
$ cat intrusiondetection.uml
$ sudo pip3 install -U plantuml
$ python3 -m plantuml intrusiondetection.uml
$ cd
$ sudo apt update
$ sudo apt install gimp pinta
$ cd ~/demo
$ pinta intrusiondetection.png
$ gimp -h
$ gimp -a intrusiondetection.png
```

![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%201.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%202.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%203.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%204.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%205.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%206.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%207.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%208.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%209.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2010.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2011.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2012.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2013.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2014.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2015.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2016.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2017.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209A%2018.png)
### intrusiondetection.png
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/intrusiondetection.png)
### GIMP
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/gimp.png)

## Lab 9B: Qiskit

```ssh
$ sudo sed -i 's/CONF_SWAPSIZE=100/CONF_SWAPSIZE=1024/' /etc/dphys-swapfile
$ sudo /etc/init.d/dphys-swapfile stop
$ sudo /etc/init.d/dphys-swapfile start
$ pip3 install setuptools-rust
$ curl -o get_rustup.sh -s https://sh.rustup.rs
$ sh ./get_rustup.sh -y
$ source ~/.cargo/env
$ pip3 install --prefer-binary retworkx
$ sudo apt -y install cmake libatlas-base-dev git
$ git clone https://github.com/sunqm/libcint.git
$ mkdir -p libcint/build && cd libcint/build
$ cmake -DCMAKE_INSTALL_PREFIX:PATH=/usr/local/ ..
$ sudo make install
$ cd
$ sudo pip3 install --prefer-binary pyscf cython
$ sudo pip3 install --prefer-binary 'qiskit[visualization]==0.23.1'
```

![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209B%201.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209B%202.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209B%203.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/4142718f4e689dcb727078f97422d0cf5a2eb992/Lab%209/Photos/Lab%209B%204.png)
Note: the lab ended here since the python example code had too many errors because of NumPy.
