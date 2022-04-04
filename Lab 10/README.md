# Lesson 10
## Lab 10A: Blockchain

```sh
$ cd ~/iot/lesson10
$ cat hash_value.py
$ python3 hash_value.py
$ python3 hash_value.py
$ python3
>>> import hashlib
>>> m = hashlib.sha256(b"hello, world")
>>> m.hexdigest()
>>> m.digest_size
>>> m.block_size
>>> exit()
$ cd ~/iot/lesson10
$ cat snakecoin.py
$ python3 snakecoin.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%201.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%202.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%203.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%204.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%205.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%206.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%207.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%208.png)

#### Terminal 1
```sh
$ cat snakecoin-server-full-code.py
$ python3 snakecoin-server-full-code.py
$ cd
```
#### Terminal 2
```sh
$ curl "localhost:5000/txion" \
     -H "Content-Type: application/json" \
     -d '{"from": "akjflw", "to":"fjlakdj", "amount": 3}'
$ curl localhost:5000/mine
```

Note: I originally got an error but this was resolved by updating Flask.

![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%209.png)

### SnakeCoin Server
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Website%201.png)

#### Terminal 1
```sh
$ git clone https://github.com/satwikkansal/python_blockchain_app.git
$ cd ~/python_blockchain_app
$ nano node_server.py
$ python3 node_server.py
```
#### Terminal 2
```sh
$ cd ~/python_blockchain_app
$ python3 run_app.py
```

![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010A%2010.png)

### Blockchain Server
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Website%202.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Website%203.png)

## Lab 10B: PyOTA
```sh
$ sudo pip3 install pyota[ccurl]
$ cd ~/iot/lesson10
$ cat iri_node_info.py
$ python3 iri_node_info.py
$ cd
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/91e8bc960eca155be0b933e3e40ffc3fa5db3993/Lab%2010/Photos/Lab%2010B%201.png)
