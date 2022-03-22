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
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/019c56e0d68eb63ec8826ec165789e3a25bfbc2c/Lab%207/Photos/Lab%207A%201.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/019c56e0d68eb63ec8826ec165789e3a25bfbc2c/Lab%207/Photos/Lab%207A%202.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/019c56e0d68eb63ec8826ec165789e3a25bfbc2c/Lab%207/Photos/Lab%207A%203.png)

### ThingSpeak cpu_loop channel
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/019c56e0d68eb63ec8826ec165789e3a25bfbc2c/Lab%207/Photos/Lab%207A%204.png)


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
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/019c56e0d68eb63ec8826ec165789e3a25bfbc2c/Lab%207/Photos/Lab%207B%201.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/019c56e0d68eb63ec8826ec165789e3a25bfbc2c/Lab%207/Photos/Lab%207B%202.png)


### Google Sheets rpidata
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/019c56e0d68eb63ec8826ec165789e3a25bfbc2c/Lab%207/Photos/Lab%207B%203.png)
