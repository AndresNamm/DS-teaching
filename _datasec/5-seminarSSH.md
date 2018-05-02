---
layout: default
title: SSH, telnet
---


# SSH tunnels

1. [This tutorial helped understanding tunneling a little]( http://www.augustcouncil.com/~tgibson/tutorial/tunneling_tutorial.html)
    + Main example is:
    ~~~
    ssh -L 8888:localhost:7180 remote.server.com
    ~~~
    In this example we assume that remote.server.com has a website available like this: remote.server.com:7180. After entering the above command we can also access this website with address localhost:8888. This is very useful when for example we cannot connect to port 7180 because of network configuration in the remote.server.com.
    + ![How this works]({{site.baseurl}}/assets/images/ssh.jpg)
2. [How signing of files/other information works](https://www.globalsign.com/en/blog/how-do-digital-signatures-work/)
3. [This information was very useful to understand ssh](https://chamibuddhika.wordpress.com/2012/03/21/ssh-tunnelling-explained/)
4. [SSH encryption description, ssh agent. Super good](http://unixwiz.net/techtips/ssh-agent-forwarding.html)
