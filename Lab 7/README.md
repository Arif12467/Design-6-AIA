# Lab 7
## Lab 7A: ThingSpeak

```ssh
$ sudo pip3 install -U psutil
$ cd ~/demo
$ cp ~/iot/lesson7/thingspeak_cpu_loop.py .
$ cp ~/iot/lesson7/thingspeak_feed.py .
$ cat thingspeak_cpu_loop.py
$ cat thingspeak_feed.py
$ python3 thingspeak_feed.py
```
![This is an image]()
![This is an image]()
![This is an image]()

### ThingSpeak cpu_loop channel
![This is an image]()


## Lab 7B: Google Sheets

```ssh
$ sudo pip3 install -U gspread oauth2client
$ cd demo
$ cp ~/iot/lesson3/system_info.py .
$ cp ~/iot/lesson7/rpi_spreadsheet.py .
$ scp rpidata-*.json pi@192.168.x.xxx:/home/pi/demo
$ nano rpi_spreadsheet.py
$ python3 rpi_spreadsheet.py
```
![This is an image]()
![This is an image]()
![This is an image]()

### Google Sheets rpidata
![This is an image]()
