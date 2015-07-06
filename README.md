# battlePyClient
Make sure to have python requests library installed. Use pip.

```
$ Pip install requests
$ git clone 'https://github.com/kevintandean/battlePyClient.git'
$ cd battlePyClient
$ touch YourPlayer.py
```
Inside YourPlayer.py must be a class inheriting from Player and must implement placeShips() and fireShot() methods. Look at RandomPlayer.py for reference.

Inside battlePyClient directory:
```
$ python
Python 2.7.6 (default, Mar 22 2014, 22:59:56)
[GCC 4.8.2] on linux2
Type "help", "copyright", "credits" or "license" for more information.
>>> import batPy
>>> batPy.register('path/to/YourPlayer.py', 'MyFirstPlayer')
...

>>> batPy.play('MyFirstPlayer', 'ImprovedRandomPlayer')
u'{"result": {"games_played": "100", "ImprovedRandomPlayer": {"win": "100"}, "MyFirstPlayer": {"win": "0"}}}'

```

batPy.register() takes filepath and name as parameters (note: name shouldn't contain file extension). Running batPy.register() will upload your file and run it against ImprovedRandomPlayer.
