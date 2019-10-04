# Cross compile for Raspberry Pi example

## Tutorial from
https://desertbot.io/blog/how-to-cross-compile-for-raspberry-pi

## Needed tools

PI Tools

https://github.com/raspberrypi/tools

## Container Details

Docker cross compile container details:

https://bitbucket.org/mitchallen/pi-cross-compile/src/master/

### Steps using the containers:

`docker pull mitchallen/pi-cross-compile`

```bash
mkdir raspberry
cd raspberry
git clone https://github.com/mitchallen/pi-hello-cross-compile.git --depth=1 hello
```

```bash
docker run -it -v ${PWD}/raspberry/hello:/build mitchallen/pi-cross-compile
ls ./hello/bin/hello
./hello/bin/hello
file  ./hello/bin/hello

```






