---
comments: false
date: 2005-09-23 16:21:24
layout: post
slug: google-has-aol-envy
title: Google has AOL envy
cover: http://farm1.static.flickr.com/14/18042843_d08c7b67f2_m.jpg
redirect_from:
 - /blog/google-has-aol-envy/
---


AOL's BYOB uses a tunnel/vpn approach.  I wonder where Google could have ever gotten the idea... but the effect is clear:

Off VPN:

```
    $ /usr/sbin/traceroute www.google.com
    traceroute: Warning: www.google.com has multiple addresses; using 64.233.161.104
    traceroute to www.l.google.com (64.233.161.104), 64 hops max, 40 byte packets
    1  192.168.1.1 (192.168.1.1)  1.984 ms  1.131 ms  1.058 ms
    2  10.47.64.1 (10.47.64.1)  6.472 ms  6.259 ms  7.544 ms
    3  srp2-0.rlghncg-rtr2.nc.rr.com (24.25.1.100)  8.038 ms  7.542 ms  8.898 ms
    4  srp4-0.rlghnca-rtr2.nc.rr.com (24.25.2.146)  8.908 ms  6.702 ms  7.779 ms
    5  pos14-0.rlghncrdc-rtr2.nc.rr.com (24.25.0.9)  9.198 ms  10.628 ms  7.281 ms
    6  son0-1-1.chrlncsa-rtr6.carolina.rr.com (24.93.64.57)  12.840 ms  12.603 ms  17.141 ms
    7  pop1-cha-p1-0.atdn.net (66.185.132.33)  14.996 ms  14.086 ms  13.759 ms
    8  bb1-cha-p3-0.atdn.net (66.185.138.64)  17.630 ms  21.680 ms  24.468 ms
    9  bb1-atm-p6-0.atdn.net (66.185.152.182)  31.240 ms  21.882 ms  20.845 ms
    10  pop2-atm-p0-0.atdn.net (66.185.147.209)  22.502 ms  16.917 ms  17.948 ms
    11  google.atdn.net (66.185.147.218)  33.378 ms  53.538 ms  29.753 ms
    12  216.239.46.153 (216.239.46.153)  28.788 ms  28.043 ms 216.239.46.157 (216.239.46.157)  30.002 ms
    13  66.249.95.125 (66.249.95.125)  30.233 ms 66.249.95.124 (66.249.95.124)  29.099 ms  29.570 ms
    14  66.249.95.123 (66.249.95.123)  30.721 ms  29.857 ms 64.233.175.98 (64.233.175.98)  43.885 ms
    15  66.249.95.121 (66.249.95.121)  40.912 ms 66.249.95.123 (66.249.95.123)  30.047 ms  29.376 ms
    16  216.239.47.156 (216.239.47.156)  37.886 ms  29.755 ms 216.239.48.198 (216.239.48.198)  36.433 ms
    17  64.233.161.104 (64.233.161.104)  28.817 ms  30.344 ms  46.271 ms
```
  

On VPN:

```  
    $ /usr/sbin/traceroute www.google.com
    traceroute: Warning: www.google.com has multiple addresses; using 66.102.7.99
    traceroute to www.l.google.com (66.102.7.99), 64 hops max, 40 byte packets
    1  * * *
    2  66.28.250.161 (66.28.250.161)  102.057 ms  99.255 ms  99.763 ms
    3  g1-8.core01.sfo01.atlas.cogentco.com (66.250.8.233)  100.255 ms  101.846 ms  100.429 ms
    4  p15-0.core02.sfo01.atlas.cogentco.com (66.28.4.70)  101.085 ms  99.884 ms  99.678 ms
    5  p10-0.core01.sjc03.atlas.cogentco.com (66.28.4.133)  101.786 ms  102.198 ms  101.599 ms
    6  google.sjc03.atlas.cogentco.com (154.54.10.254)  102.646 ms  102.553 ms  101.197 ms
    7  66.249.94.2 (66.249.94.2)  175.315 ms  176.190 ms  180.260 ms
    8  64.233.174.54 (64.233.174.54)  177.706 ms  176.194 ms 66.249.94.29 (66.249.94.29)  176.665 ms
    9  216.239.49.142 (216.239.49.142)  176.362 ms  177.084 ms 216.239.49.146 (216.239.49.146)  176.446 ms
    10  66.102.7.99 (66.102.7.99)  175.962 ms  177.078 ms  175.809 ms
```
