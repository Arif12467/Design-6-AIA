# Lab 5
## Lab 5B: Eclipse Mosquitto and Eclipse Paho
### Eclipse Mosquitto
```ssh
$ sudo apt update
$ sudo apt install mosquitto mosquitto-clients
$ mosquitto_sub -h localhost -v -t "\$SYS/#"
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/1a306a8486fa4e6548d908fa3425920ba91fb620/Lab%205/Photos/mosquitto_install.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/1a306a8486fa4e6548d908fa3425920ba91fb620/Lab%205/Photos/mosquitto_install_1.png)


```ssh
$ service mosquitto status
$ netstat -tln
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/1a306a8486fa4e6548d908fa3425920ba91fb620/Lab%205/Photos/service-netstat.png)


Terminal 1
```sh
$ mosquitto_sub -h localhost -v -t test/topic &
```
Terminal 2
```sh
$ mosquitto_pub -h localhost -t test/topic -m "Hello"
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/1a306a8486fa4e6548d908fa3425920ba91fb620/Lab%205/Photos/mosquitto_run.png)


### Eclipse Paho
```sh
$ sudo pip3 install -U paho-mqtt
$ git clone https://github.com/eclipse/paho.mqtt.python.git
$ cd ~/iot/lesson5
$ python3 client.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/1a306a8486fa4e6548d908fa3425920ba91fb620/Lab%205/Photos/paho_install.png)


Terminal 1 
```sh
$ python3 sub.py
$ python3 sub-multiple.py
$ python3 subcpu.py
```
Terminal 2
```sh
$ python3 pub.py
$ python3 pub-multiple.py
$ python3 pubcpu.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/1a306a8486fa4e6548d908fa3425920ba91fb620/Lab%205/Photos/paho_run.png)
