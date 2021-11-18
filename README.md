# xrd-ospf-triangle-sarimits

# Topology
```
      source
       |
      xrd1
     /    \
  xrd2 -- xrd3-server
   |
  dest
```
# Networks


host (172.28.0.1/16): xrd1 172.28.0.10, xrd2 172.28.0.20, xrd3 172.28.0.30
source-xrd1 (192.168.1.0/24):  192.168.1.2 - 192.168.1.254 (source - Gi0/0/0/0)
dest-xrd2 (192.168.2.0/24):  192.168.2.2 - 192.168.2.254 (dest - Gi0/0/0/2)
xrd1-xrd2 (10.0.1.0/24):  10.0.1.2 - 10.0.3.3 (Gi0/0/0/1 - Gi0/0/0/0)
xrd1-xrd3 (10.0.2.0/24):  10.0.2.2 - 10.0.2.3 (Gi0/0/0/2 - Gi0/0/0/0)
xrd2-xrd3 (10.0.3.0/24):  10.0.3.2 - 10.0.3.3 (Gi0/0/0/1 - Gi0/0/0/2)

Author: sarimits
