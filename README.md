MySQL Shell Innotop
===================

This is a Innotop like Python module for MySQL Shell.

How to use it:
--------------

```
 mysqlsh --py root@localhost           <<<--- connect to the X console otherwise the global classes won't be found: root@localhost:33060

 import sys
 sys.path.append('/home/fred/workspace/mysql-shell-innotop')
 import innotop

 innotop.session_processlist.run()
``` 

It's also possible to add some steps in *~/.mysqlsh/mysqlshrc.py*:

```
 import sys
 sys.path.append('/home/fred/workspace/mysql-shell-innotop')
 import innotop
```

and then in the Shell, just call _innotop.session_processlist.run()_ 

https://youtu.be/QFgSPxZm9CY
