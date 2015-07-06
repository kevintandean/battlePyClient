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
>>> import batPy

>>> batPy.register('path/to/YourPlayer.py', 'MyFirstPlayer')
>>> batPy.play('SomePlayer', 'MyFirstPlayer')
```

batPy.register() takes filepath and name as parameters (note: name shouldn't contain file extension). Running batPy.register() will upload your file and run it against ImprovedRandomPlayer.
