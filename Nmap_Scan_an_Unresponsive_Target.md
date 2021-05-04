###### Use of nmap will not be documented much here, as full documentation exists at https://nmap.org . This is here because it's quick information that could be needed in actual practice.
# Nmap port scanning a target that is unresponsive and gives little information

When in reconiassance and port scanning using nmap, the status of ports may return `filtered` or `tcpwrapped` instead of simply `open` or `closed`. If so then this is because the target's networking has been strictly configured. Nmap uses numerous TCP trickery techniqes and 'SYN' scanning by default. In this type of scan, nmap does not complete the TCP connection. Many of the previously mentioned security technologies have ways of protecting themselves from such recon methods however. Despite this, there are some basic things that cannot be restricted and that could even cripple the device's networking capability.

Full TCP connections cannot be blocked or restricted because that would be stripping the device of a basic networking ability, if it has been restricted in this manner then it barely has any networkability and should not be further pursued. All of nmap's TCP techniqes including the default opt to do anything but this. However it can still do full TCP connects if specified, using `-sT`.

Pings AKA ICMP probes may be turned off. Nmap does this by default to see if the host is up. If the targets ping response is turned off then nmap will not scan correctly. Ping probing may be turned off with `-Pn`.

###### https://nmap.org/book/man-port-scanning-techniques.html
###### https://nmap.org/book/man-bypass-firewalls-ids.html
