# Cross compile for Raspberry Pi example

## Tutorial from
https://desertbot.io/blog/how-to-cross-compile-for-raspberry-pi

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






