```
           ▓█████▄  ██▓  ██████  ▄████▄   ▒█████   ██▀███  ▓█████▄             
           ▒██▀ ██▌▓██▒▒██    ▒ ▒██▀ ▀█  ▒██▒  ██▒▓██ ▒ ██▒▒██▀ ██▌            
           ░██   █▌▒██▒░ ▓██▄   ▒▓█    ▄ ▒██░  ██▒▓██ ░▄█ ▒░██   █▌            
           ░▓█▄   ▌░██░  ▒   ██▒▒▓▓▄ ▄██▒▒██   ██░▒██▀▀█▄  ░▓█▄   ▌            
           ░▒████▓ ░██░▒██████▒▒▒ ▓███▀ ░░ ████▓▒░░██▓ ▒██▒░▒████▓             
            ▒▒▓  ▒ ░▓  ▒ ▒▓▒ ▒ ░░ ░▒ ▒  ░░ ▒░▒░▒░ ░ ▒▓ ░▒▓░ ▒▒▓  ▒             
            ░ ▒  ▒  ▒ ░░ ░▒  ░ ░  ░  ▒     ░ ▒ ▒░   ░▒ ░ ▒░ ░ ▒  ▒             
            ░ ░  ░  ▒ ░░  ░  ░  ░        ░ ░ ░ ▒    ░░   ░  ░ ░  ░             
              ░     ░        ░  ░ ░          ░ ░     ░        ░                
              ░              ░                                ░                  
     ███▄ ▄███▓▓██   ██▓  ██████   █████   ██▓       ▓█████▄  ███▄ ▄███▓
    ▓██▒▀█▀ ██▒ ▒██  ██▒▒██    ▒ ▒██▓  ██▒▓██▒       ▒██▀ ██▌▓██▒▀█▀ ██▒
    ▓██    ▓██░  ▒██ ██░░ ▓██▄   ▒██▒  ██░▒██░       ░██   █▌▓██    ▓██░
    ▒██    ▒██   ░ ▐██▓░  ▒   ██▒░██  █▀ ░▒██░       ░▓█▄   ▌▒██    ▒██ 
    ▒██▒   ░██▒  ░ ██▒▓░▒██████▒▒░▒███▒█▄ ░██████▒   ░▒████▓ ▒██▒   ░██▒
    ░ ▒░   ░  ░   ██▒▒▒ ▒ ▒▓▒ ▒ ░░░ ▒▒░ ▒ ░ ▒░▓  ░    ▒▒▓  ▒ ░ ▒░   ░  ░
    ░  ░      ░ ▓██ ░▒░ ░ ░▒  ░ ░ ░ ▒░  ░ ░ ░ ▒  ░    ░ ▒  ▒ ░  ░      ░
    ░      ░    ▒ ▒ ░░  ░  ░  ░     ░   ░   ░ ░       ░ ░  ░ ░      ░   
           ░    ░ ░           ░      ░        ░  ░      ░           ░   
                ░ ░                                   ░                 

```
Make sure your working on a server or computer with mySQL and Python3  installed # [GitHub](http://github.com),# [Python3](https://www.python.org/downloads/)


> ### First you must install the dependencies:

```bash
$- pip3 install -r requirements.txt
```

> ### Edit the config.py:
```
001   host = "localhost"
002   user = "root"
003   pswd = "root"
004   dbse = "sqltodisc"
005   port = 3306
006   acmt = True
```

>  Next open the send.py and verify `line 102` the table is the correct name (currently ***dm_users****):
```bash
100  	
101  	cursor1 = db.cursor()
102   cursor1.execute("select * from dm_users where robot='0' ORDER BY id DESC")
103  	usersResult = cursor1.fetchall()
104           
105   indx = 0  
  
```  
>  Next scroll down and edit `line 124` and swap your discord [TokenHere]:
```
bot.run("[TokenHere]", bot = False)TokenHere]
```

run **send.py** 
```bash
$- python3 send.py
```


###### If any errors occor your working on a server or computer with mySQL v5.7 and/or python version 3.6



###### Created by CodeInFilth
