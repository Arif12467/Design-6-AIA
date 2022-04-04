# Lesson 10
## Lab 10A: Blockchain
```sh
$ cd ~/iot/lesson10
$ cat hash_value.py
$ python3 hash_value.py
$ python3 hash_value.py
```

```sh
$ python3
>>> import hashlib
>>> m = hashlib.sha256(b"hello, world")
>>> m.hexdigest()
>>> m.digest_size
>>> m.block_size
>>> exit()
```

```sh
$ cd ~/iot/lesson10
$ cat snakecoin.py
$ python3 snakecoin.py
```

### Terminal 1
```sh
$ cat snakecoin-server-full-code.py
$ python3 snakecoin-server-full-code.py
$ cd
```
### Terminal 2
```sh
$ curl "localhost:5000/txion" \
     -H "Content-Type: application/json" \
     -d '{"from": "akjflw", "to":"fjlakdj", "amount": 3}'
$ curl localhost:5000/mine
```


### Terminal 1
```sh
$ git clone https://github.com/satwikkansal/python_blockchain_app.git
$ cd ~/python_blockchain_app
$ nano node_server.py
$ python3 node_server.py
```
### Terminal 2
```sh
$ vncserver
$ cd ~/python_blockchain_app
$ python3 run_app.py
```

## Lab 10B: PyOTA
```sh
$ sudo pip3 install pyota[ccurl]
$ cd ~/iot/lesson10
$ cat iri_node_info.py
$ python3 iri_node_info.py
$ cd
```
