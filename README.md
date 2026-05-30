# Task 1: Scan Your Local Network for Open Ports

## Objective

The objective of this task was to discover active devices and identify open ports on a local network using Nmap.

## Tools Used

* Nmap 7.99
* Windows Command Prompt

## Network Information

* IPv4 Address: 10.250.208.76
* Subnet Mask: 255.255.255.0
* Default Gateway: 10.250.208.77
* Network Range: 10.250.208.0/24

## Command Executed

```bash
nmap -sS 10.250.208.0/24
```

## Results

### Host 1

IP Address: 10.250.208.77

Open Port:

* 53/tcp (DNS)

### Host 2

IP Address: 10.250.208.76

Open Ports:

* 135/tcp (MSRPC)
* 139/tcp (NetBIOS)
* 445/tcp (SMB)

## Security Findings

* Port 53 is used for DNS services.
* Port 135 is used by Microsoft RPC services.
* Port 139 is used for NetBIOS file sharing.
* Port 445 is used for SMB file sharing.


## Conclusion

The network scan successfully identified active hosts and open ports on the local network. Standard Windows networking services were found running on the local machine, while DNS services were discovered on the gateway device.
