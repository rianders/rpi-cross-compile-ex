# Cross compile for Raspberry Pi example

## Tutorial from
https://desertbot.io/blog/how-to-cross-compile-for-raspberry-pi

`docker pull mitchallen/pi-cross-compile`

```
mkdir raspberry
git clone https://github.com/mitchallen/pi-hello-cross-compile.git --depth=1 hello
```

```
docker run -it -v /Users/rianders/Documents/projects/rianders/rpi-cross-compile/raspberry/hello:/build mitchallen/pi-cross-compile
ls ./hello/bin/hello
./hello/bin/hello
file  ./hello/bin/hello

```






