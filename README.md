# pcap-test
Packet Capture Application

## usage
```shell
ugonfor@gongon:~/ugonfor/pcap-test$ make
g++    -c -o pcap-test.o pcap-test.cpp
g++   pcap-test.o main.o  -lpcap -o pcap-test
ugonfor@gongon:~/ugonfor/pcap-test$ sudo ./pcap-test eth0
```

## example
```shell
==================================================
ether_type: 0x0800
ip_protocol: 0x06
TCP Packet Captured

Ethernet II
        Src MAC: aa:bb:cc:dd:ee:ff
        Dst MAC: aa:bb:cc:dd:ee:ff
IP Datagram
        Src IP: 1.2.3.4
        Dst IP: 1.2.3.4
TCP Segment
        Src Port: 443
        Dst Port: 443

Data size: 0
Memory Dump
      00 01 02 03 04 05 06 07 08 09 0a 0b 0c 0d 0e 0f  0123456789ABCDEF
0x00  15 03 03 00 1a 48 df 24 

54 bytes captured
```