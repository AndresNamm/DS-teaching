---
layout: default
title: SSH, telnet
---


# SSH tunnels

1. [this helped a little]( http://www.augustcouncil.com/~tgibson/tutorial/tunneling_tutorial.html)
    + Main example is:
    ~~~
    ssh -L 8888:localhost:7180 remote.server.com
    ~~~
    In this example we assume that remote.server.com has a website available like this: remote.server.com:7180. After entering the above command we can also access this website with address localhost:8888. This is very useful when for example we cannot connect to port 7180 because of network configuration in the remote.serve.com.
2. [How signing of files/other information works](https://www.globalsign.com/en/blog/how-do-digital-signatures-work/)
