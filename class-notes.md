## 10 oct 2024

OSI reference model

## 15 oct 2024

Ethernet frames are local. They are discarded oh the first hop. 

### Encapsulation example

L7 -> message : D (dns) | google.com

L4 -> segments. UDP can also be called datagram : U | D google

L3 -> packets : I | U D google.com

L2 -> frame : W (wi-fi header) | I U D google.com | T (trailing with hashsum)

L1 -> bits on 

Anycast -> how famous IP's like 8.8.8.8 use "reverse proxy"

DNS messages are usually transfered via UDP