# battlePyClient
Make sure to have python requests library installed. Use pip.

```
$ Pip install requests
$ git clone 'https://github.com/kevintandean/battlePyClient.git'
$ cd battlePyClient
$ touch YourPlayer.py
```
Inside YourPlayer.py must be a player object inheriting from Player, look at RandomPlayer.py for reference.

Inside battlePyClient directory:
```
$ python
>>> import batPy

>>> batPy.register('YourPlayer.py', 'MyFirstPlayer')
>>> batPy.play('SomePlayer', 'MyFirstPlayer')
```

Running batPy.register() will upload your file and run it against ImprovedRandomPlayer.
