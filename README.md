# scapy-tools
anaylyze network packets in kali linux with scapy tool
SCAPY tool in KALI Linux
sudo apt update
sudo apt install scapy -y

sudo apt install python3-pip -y
pip3 install scapy

from scapy.all import *
>>> file = rdpcap('Dns.cap')

>file
>file.show()
>f = file[0]
>f.show()
>f[DNS=protocol].id
>f[DNS=protocol].id = 123456
>p = IP(dst='1.2.3.4')/UDP(dport=1234)/DNS()
>p.show()

