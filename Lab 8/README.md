# Lab 8
## Lab 8A: Examples

```ssh
$ sudo apt update
$ sudo apt install python3-scipy
$ sudo apt install python3-matplotlib
$ sudo apt install python3-pandas
$ sudo apt install libopenblas-dev
$ sudo apt install libatlas-base-dev
$ sudo pip3 install -U numpy
$ sudo pip3 install --only-binary :all: -U scikit-learn
$ sudo pip3 install -U tensorflow
$ sudo pip3 install -U keras==2.3.1
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%201.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%202.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%203.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%204.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%205.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%206.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%207.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%209.png)


### Titanic Example
```ssh
$ cp train.csv ~/demo
$ cp test.csv ~/demo
$ cp titanic_1.py ~/demo
$ cp titanic_2.py ~/demo
$ cd ~/demo
$ python3 titanic_1.py
$ python3 titanic_2.py
```
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208A%20titanic.png)

### Number of Passengers vs Passengers Class Figure
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Figure_1_titanic.png)


## Lab 8B: Data Analysis

```ssh
$ cd ~/demo
$ cp ~/iot/lesson8/plt_final.py .
$ cp ~/iot/lesson8/plt_cv2.py .
$ nano plt_final.py
$ nano plt_cv2.py
$ python3 plt_final.py
$ python3 plt_cv2.py 
```
Note: Error with $ python3 plt_cv2.py

Resolved: Updated NumPy, SciPy, NumExpr, and pandas. Additional modified plt_cv2.py line 11 from cv=10 to cv=9.

![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/881f3979a13f928acd4b0837c5fa3374d19f3dd7/Lab%208/Photos/Lab%208B%201.png)

### Figures
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d3d372ce349950aabd75fd9b3070ee492e047292/Lab%208/Photos/L8Figure_1.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d3d372ce349950aabd75fd9b3070ee492e047292/Lab%208/Photos/L8Figure_2.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d3d372ce349950aabd75fd9b3070ee492e047292/Lab%208/Photos/L8Figure_3.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d3d372ce349950aabd75fd9b3070ee492e047292/Lab%208/Photos/L8Figure_4.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d3d372ce349950aabd75fd9b3070ee492e047292/Lab%208/Photos/L8Figure_5.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d3d372ce349950aabd75fd9b3070ee492e047292/Lab%208/Photos/L8Figure_6.png)
![This is an image](https://github.com/Arif12467/Design-6-AIA/blob/d3d372ce349950aabd75fd9b3070ee492e047292/Lab%208/Photos/L8Figure_7.png)
