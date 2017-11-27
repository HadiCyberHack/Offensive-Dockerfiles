# Gitminer

![Screenshot](https://3.bp.blogspot.com/-UvpR_QDDAT0/VtiIc8OKrrI/AAAAAAAAboM/69BNKrvdUsU/s1600/gitminer-628x360.png)


## Source 
http://github.com/danilovazb

## Usage 
```bash
cd gitminer/
docker build -t gitminer .
docker run -it gitminer:latest
```



## Help
```
 ██████╗ ██╗████████╗███╗   ███╗██╗███╗   ██╗███████╗██████╗
██╔════╝ ██║╚══██╔══╝████╗ ████║██║████╗  ██║██╔════╝██╔══██╗
██║  ███╗██║   ██║   ██╔████╔██║██║██╔██╗ ██║█████╗  ██████╔╝
██║   ██║██║   ██║   ██║╚██╔╝██║██║██║╚██╗██║██╔══╝  ██╔══██╗
╚██████╔╝██║   ██║   ██║ ╚═╝ ██║██║██║ ╚████║███████╗██║  ██║
 ╚═════╝ ╚═╝   ╚═╝   ╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝ v1.1
 Automatic search for GitHub.

 + Autor: Danilo Vaz a.k.a. UNK
 + Blog: http://unk-br.blogspot.com
 + Github: http://github.com/danilovazb
 + Gr33tz: l33t0s, RTFM

 +[WARNING]------------------------------------------+
 | DEVELOPERS ASSUME NO LIABILITY AND ARE NOT        |
 | RESPONSIBLE FOR ANY MISUSE OR DAMAGE CAUSED BY    |
 | THIS PROGRAM                                      |
 +---------------------------------------------------+


       [-h] [-q 'filename:shadow path:etc']
       [-m wordpress] [-o result.txt]
       [-c pAAAhPOma9jEsXyLWZ-16RTTsGI8wDawbNs4]

optional arguments:
  -h, --help            show this help message and exit
  -q 'filename:shadow path:etc', --query 'filename:shadow path:etc'
                        Specify search term
  -m wordpress, --module wordpress
                        Specify the search module
  -o result.txt, --output result.txt
                        Specify the output file where it will be
                        saved
  -c pAAAhPOma9jEsXyLWZ-16RTTsGI8wDawbNs4, --cookie pAAAhPOma9jEsXyLWZ-16RTTsGI8wDawbNs4
                        Specify the cookie for your github
```

### EXAMPLE
Searching for wordpress configuration files with passwords:
```
$:> python git_miner.py -q 'filename:wp-config extension:php FTP_HOST in:file ' -m wordpress -c pAAAhPOma9jEsXyLWZ-16RTTsGI8wDawbNs4 -o result.txt
```
![Screenshot](https://2.bp.blogspot.com/-GbpzROiEynQ/VtLytfMqQiI/AAAAAAAAbnk/5hDphP4Mbf4/s1600/wordpressEX.png)

Looking for brasilian government files containing passwords:
```
$:> python git_miner.py --query 'extension:php "root" in:file AND "gov.br" in:file' -m senhas -c pAAAhPOma9jEsXyLWZ-16RTTsGI8wDawbNs4
```

Looking for shadow files on the etc paste:
```
$:> python git_miner.py --query 'filename:shadow path:etc' -m root -c pAAAhPOma9jEsXyLWZ-16RTTsGI8wDawbNs4
```

Searching for joomla configuration files with passwords:
```
$:> python git_miner.py --query 'filename:configuration extension:php "public password" in:file' -m joomla -c pAAAhPOma9jEsXyLWZ-16RTTsGI8wDawbNs4
```
![Screenshot](https://3.bp.blogspot.com/-1AsNmFKfsoA/VtLyvJFy2WI/AAAAAAAAbno/C7xTbxtzOo8/s1600/joomlaEX.png)

### Hacking SSH Servers

[![Hacking SSH Servers](https://img.youtube.com/vi/yIJOlKZwQQw/0.jpg)](https://www.youtube.com/watch?v=yIJOlKZwQQw)
