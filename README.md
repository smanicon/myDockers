My Docker
=========

##Docker CNC :

to build image :
```shel
$ docker build -t cnc -f cncDockerFile .
```

to execute image:
```shell
$ docker run --rm -ti --device="/dev/ttyACM0" --env="DISPLAY" --net="host" --volume="$HOME/.Xauthority:/root/.Xauthority:rw" --volume="$HOME/Documents:/home/cnc/Documents" cnc
```

