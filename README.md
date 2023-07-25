# Python Multithreaded Port Scanner

This port scanner utilizes multithreading in Python to achieve very fast scan speeds. It can scan a wide range of ports on any IPv4 address.

## Features

- Multithreaded design for incredibly fast scan speeds
  - Can scan thousands of ports per second
  - Adjustable number of threads for optimizing performance
- Scan any range of ports
  - Specify starting and ending port numbers
  - Scans most common ranges in seconds
- Target any IPv4 address or hostname
  - Scan local or external IPs and hosts
- Verbose output shows open ports in real-time
  - See results as they are found, no waiting until the end
  - Great for monitoring progress during longer scans
- Lightweight Python script without dependencies
  - Runs on all major platforms
  - Easy to modify or integrate into other tools

## Usage

The scanner accepts the following command line arguments:
- ```-h, --help```= Show help message and exit      
- ```-V, --ip```= IP address to target for scanning
- ```-s, --start```= Starting port number (default 1)
- ```-e, --end```= Ending port number (default 65535)
- ```-t, --threads```= Number of threads to use (default 500)
- ```-V, --verbose```= Verbose output showing open ports

## Installation 
### Clone Repository:
```
git clone https://github.com/satharv/Port-Scanner-Python
```
### Unzip and run:
```
cd Port-Scanner-Python-main
```

### To scan ports 1-65535 on 192.168.1.100 with 200 threads:
```
python portscanner.py -V 192.168.1.100 -t 200
```

### To scan a smaller range with verbose output:
```
python portscanner.py -V 192.168.1.100 -s 1 -e 1000 -V
```
The verbose output will print open ports to the screen as they are discovered.
