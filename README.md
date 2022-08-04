<h2>Description</h2>

Optimized nmap scan useful for pentesting, ctfs, etc

<h2>Features</h2>

<h4>Default mode</h4>

- initial os discovery based on ping ttl
- scans all 65535 tcp ports then performs targeted service scan based on open ports
- saves results to output file

<h4>Proxy mode</h4>

- for scanning targets in other networks behind a proxy (ie pivoting)
- integrates proxychains to scan common ports, then performs targeted service scan based on open ports
- for best results comment out "proxy_dns" in /etc/proxychains.conf
- saves results to output file

<h4>Range mode</h4>

- for scanning network ranges
- finds alive hosts on network using fping
- for each host, scans all ports then performs targeted service scan based on open ports
- saves results to output file
- can be very slow

<h2>Options</h2>

```
usage: p0rtscan [-d] [-p] [-r] addr

optimized nmap scan useful for pentesting, ctfs, etc

options:
  -d	default scan
  -p	proxy scan
  -r	range scan (slow)

```
