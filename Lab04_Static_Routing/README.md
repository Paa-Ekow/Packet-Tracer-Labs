README
# Lab 04: Static Routing 

## Objective
Connect two separate LANs using two routers to form static connection and verify inter-network communication.

## Topology
![Topology](topology.png)

## IP Addressing

### LAN 1
- Network: 192.168.1.0/24
- Gateway: 192.168.1.1

### LAN 2
- Network: 192.168.2.0/24
- Gateway: 192.168.2.1

## Router 1 Configuration
- G0/0: 192.168.1.1
- G0/1: 10.0.0.1 (WAN Link)

## Router 2 Configuration
- G0/0: 192.168.2.1
- G0/1: 10.0.0.2 (WAN Link)

## IP Routing on Router 1
- ip route 192.168.2.0 255.255.255.0 10.0.0.2

## IP Routing on Router 2
- ip route 192.168.1.0 255.255.255.0 10.0.0.1

## Verification
- Successful ping between LANs

## Lessons Learned
- Static routing enable communication between different networks
- One router interface connects to one LAN and the other connects to a WAN Link 

## Full Documentation
👉 [Google Drive – Lab 04 Documentation](https://drive.google.com/file/d/1C6xajFWRwwPF299ud6Y0rQqe9muUbaul/view?usp=sharing)
