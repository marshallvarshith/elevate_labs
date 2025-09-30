Capture and Analysis of Network packet using wireshark

Wireshark is extensively used to capture and analyze network traffic by all security professionals, it gives access to detailed information of packets and transmission data between two endpoints.
details like destination port, source port, destination ip, source ip, amount of data transferred can be obtained. it also give you protocol filter and other commands.

step 1:
install wireshark on your local machine

sudo apt install wireshark -y

step 2:
open wireshark and start on your network interface

step 3:
generate traffic by browsing any website for example: google.com

step 4:
stop wireshark and use tcp, http, dns filter on the filter column in wireshark to analyze searched protocol

step 5:
export the packet analysis .pcap file

commands:

ip.add == 10.10.50.1
ip.dest == 10.10.50.1
ip.src == 10.10.50.1
tcp.port == 25

files included:

1. t5_basic_scan_eth1.pcapng
2. t5_dns_filter.png
3. t5_http_filter.png
4. t5_tcp_filter.png
