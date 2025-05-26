## Scan Local Network for Open Ports

## Using nmap
  Linux operating system used
  In Linux operating system,
  1. Using, **ifconfig** find out the ip address.
  2. **nmap -sS ip_address/24** : for TCP SYN scan, this will list the active devices and their open ports.
  3. **nmap -T4 -sS ip_address/24**: for faster scanning.
  4. **nmap -A -T4 -sS ip_address/24** : for aggressive scanning.
  5. **nmap -sS -sV -O ip_address/24** :
       -sV for service version and -O for Operating system detection.
 6. **nmap -sS -sV -O ip_address/24 -oN nmap_scanning.txt** : saved this report as nmap_scanning and using .txt format.
## Using wireshark
    Wireshark is packet capturing tool. It capture packets real-time.
    Captured packets can be analysed, we can get the information like ip address, host information, if the site is not decured we can get the login information, hex decimal inside the packets
