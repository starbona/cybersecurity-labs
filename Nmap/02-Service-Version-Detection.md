# Lab 02 - Service Version Detection (-sV)

## Objective

Identify the services running on open ports and determine their versions.

## Command Used

```bash
sudo nmap -sV example.com
```

## What the command does

The `-sV` option tells Nmap to perform service version detection on open ports.

Instead of only identifying that a port is open, Nmap attempts to determine the exact service running behind that port.

## Observations

The scan identified several open ports, including:

- Port 80 (HTTP)
- Port 443 (HTTPS)
- Cloudflare HTTP Proxy
- SSL/HTTP services

Many other ports appeared as **tcpwrapped**, meaning the services accepted the TCP connection but restricted further interaction.

## Key Findings

- Host was reachable.
- Multiple services were identified.
- HTTP and HTTPS were protected by Cloudflare.
- Service detection provides more information than a normal port scan.

## Skills Practiced

- Service Enumeration
- Port Analysis
- Nmap Version Detection
- Network Reconnaissance

## Screenshot

(Add your -sV screenshot here.)

## Lessons Learned

Knowing that a port is open is only the first step.

Service version detection helps identify the actual applications running behind those ports, making vulnerability assessment more effective.
