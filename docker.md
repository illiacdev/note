***
## snap docker 설정

systemctl edit snap.docker.dockerd

~~~
[Service]
ExecStart=
ExecStart=/usr/bin/snap run docker.dockerd  -H unix:// -H tcp://0.0.0.0:2376
~~~