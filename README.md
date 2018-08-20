Ping Pong with Socat
============

Description:
-----------

Three machines setup, two VMs and one host.

On each VM we ask socat to forward a specific port to the other VM,

We also ask it to wait two seconds before running it, and we can see with tcpdump when the packets are recived.

At the fourth hop socat runs "echo Hey", that we can see on the host machine (on the left side)


How to run:
-----------

$ scriptreplay --timing=./time-socat.log ./socat.log


Bugs:
-----------

I am missing "$ iptables -F" on one of the Vms, it's just something I did earlier that wasn't recorded
