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

<h2>Options</h2>

```
usage: p0rtscan [-d] [-p] host

optimized nmap scan useful for pentesting, ctfs, etc

options:
  -d	default scan
  -p	proxy scan

```
