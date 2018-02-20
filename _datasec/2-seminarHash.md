---
title: "Cryptography"
modified: 2017-08-01T15:54:02-04:00
---



# Main
## Hash functions
+ [Hash functions meaning ](https://www.youtube.com/watch?v=--tnZMuoK3E)
+ [Hash functions meaning 2](https://www.youtube.com/watch?v=a5F16sM75uY)
+ [hashs functions properties](https://denimgroup.com/resources/blog/2007/11/properties-of-1/)
## Practical example why hash is necessary
+ [Java code to perform md5 hashing - you have to remove the salt](http://www.codexpedia.com/java/java-md5-hash-example-one-way-hash/)
+ [Hash function database for md5](https://hashkiller.co.uk/md5-decrypter.aspx)
+ hash of word "password"
~~~
5f4dcc3b5aa765d61d8327deb882cf99
~~~
+ [Linux Mint set hash function location](https://unix.stackexchange.com/questions/196085/how-to-set-default-password-algorithm-to-sha512-on-linux)
~~~
/etc/login.defs
~~~

+ linux lcrypt example
+ crypt function first parameter -  password chosen
+ crypt function second parameter - $<key>$salt
+ In this case
    + password - password1
    + key - 1 (means md5)
    + salt - NBSmdW0E
+ result - $1$NBSmdW0E$PTcjork/6DMui1ogc2g/0.
~~~
#define _XOPEN_SOURCE
#include <unistd.h>
#include <stdio.h>


int main() {
    printf("%s\n", crypt("password1","$1$NBSmdW0E"));
}
~~~

## Cracking  passwords with John

+ [Tutorial 1](https://linuxconfig.org/password-cracking-with-john-the-ripper-on-linux)
+ [Tutorial 2](https://gbhackers.com/offline-password-attack-john-ripper/)
+ [Good tutorial about Cracking modes with John](http://www.openwall.com/john/doc/MODES.shtml)
    + [John examples](http://www.openwall.com/john/doc/EXAMPLES.shtml)


## PROXY

+ [Simple explanation](https://www.whatismyip.com/what-is-a-proxy/)

# If you are very interested

+ This tutorial involves understanding the booting process very thoroughly. It involves crypting the hardrive and setting up the booting manually to work with the encrypted harddrive.
[System Administration practical 2](https://courses.cs.ut.ee/2018/sa/spring/Main/Bootstrapping)
