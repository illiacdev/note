***
###
WSL2 remote access

https://www.brianketelsen.com/ssh-to-wsl2/

~~~
netsh interface portproxy add v4tov4 listenport=2222 listenaddress=0.0.0.0 connectport=2222 connectaddress=172.19.149.102
~~~
