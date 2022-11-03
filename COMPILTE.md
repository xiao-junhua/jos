# Compile 
[related links](https://pdos.csail.mit.edu/6.828/2018/tools.html)
1. Cannot clone the project.
The basic reason is that your computer doesn’t trust the certificate authority that signed the certificate used on the Gitlab server. 
Just add an environment variables.  
```bash
$ export GIT_SSL_NO_VERIFY=1
```
2. Install python2
```bash
sudo apt install python-is-python2
```
3. zlib check failed
```bash
sudo apt install zlib1g-dev
```
4. glib-2.12 etc
```bash
sudo apt install libglib2.0-dev
```
5. pixman
```bash
sudo apt install libpixman-1-dev
```
6. libtool missing -> install all libtool-related libs
```bash
sudo apt install libtool*
```
7. libtool disabled ...
```bash
sudo apt install libtool-bin```
8. undefined reference to `major`
add following line to code:
```c
#include <sys/types.h>
#include <sys/sysmacros.h>```
