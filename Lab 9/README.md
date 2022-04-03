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

![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()

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

![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
![This is an image]()
Note: ```ssh $ sudo pip3 install --prefer-binary 'qiskit[visualization]==0.23.1'``` failed and the lab ended here
