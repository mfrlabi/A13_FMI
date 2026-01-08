# A13_FMI

    labi@lb:~$ ssh root@192.168.10.1

    labi@lb:~$ ssh-keygen -f '/home/labi/.ssh/known_hosts' -R '192.168.10.1'

    labi@lb:~$ ssh root@192.168.10.1


CXa13sadmin


    root@MERCURYNAVIRK3588:~# cd /cxapp/ssd/data/
    root@MERCURYNAVIRK3588:/cxapp/ssd/data#


    root@MERCURYNAVIRK3588:/cxapp/ssd/data# ls
data_2025-12-16-19-15-24  data_2025-12-17-14-42-44
data_2025-12-17-14-41-21  data_2025-12-17-16-58-16
   
    root@MERCURYNAVIRK3588:/cxapp/ssd/data# 


    root@MERCURYNAVIRK3588:/cxapp/ssd/data# rsync -avz data_2025-12-17-14-41-21 data_2025-12-17-14-42-44 labi@192.168.10.227:/home/labi/ws_livox/a13/

 ------------------------------------------------------------------------



2nd Terminal:
 
    labi@lb:~$ ifconfig
     
enx00e04c253008: flags=4099<UP,BROADCAST,MULTICAST>  mtu 1500
        ether 00:e0:4c:25:30:08  txqueuelen 1000  (Ethernet)
        RX packets 0  bytes 0 (0.0 B)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 0  bytes 0 (0.0 B)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

lo: flags=73<UP,LOOPBACK,RUNNING>  mtu 65536
        inet 127.0.0.1  netmask 255.0.0.0
        inet6 ::1  prefixlen 128  scopeid 0x10<host>
        loop  txqueuelen 1000  (Local Loopback)
        RX packets 1623519  bytes 1194394569 (1.1 GB)
        RX errors 0  dropped 0  overruns 0  frame 0
        TX packets 1623519  bytes 1194394569 (1.1 GB)
        TX errors 0  dropped 0 overruns 0  carrier 0  collisions 0

wlo1: flags=4163<UP,BROADCAST,RUNNING,MULTICAST>  mtu 1500
        inet 192.168.10.227  netmask 255.255.255.0  broadcast 192.168.10.255
        inet6 fe80::2cb6:fcab:6998:7c6b  prefixlen 64  scopeid 0x20<link>
        ether c8:a3:e8:ad:07:c5  txqueuelen 1000  (Ethernet)
        RX packets 4344170  bytes 5711218391 (5.7 GB)
        RX errors 0  dropped 23124  overruns 0  frame 0
        TX packets 1174544  bytes 228567321 (228.5 MB)
        TX errors 0  dropped 226 overruns 0  carrier 0  collisions 0

labi@lb:~$ 



192.168.10.227

---------------------------------------------------------------------------------------






http://192.168.10.1:5000

if you change the wifi 

http://192.168.101.33:5000


Transfer data from PC to A13

labi@lb:~/ws_livox/a13$ rsync -avz data_2025-12-17-16-58-16 root@192.168.10.1:/cxapp/ssd/data/

CXa13sadmin
