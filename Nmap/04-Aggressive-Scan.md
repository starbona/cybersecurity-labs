# Lab 04 - Aggressive Scan (-A)

## Objective

Perform a comprehensive scan to gather detailed information about the target host, including operating system, running services, default scripts, and network path.

## Command Used

```bash
sudo nmap -A example.com
```

## What the command does

The `-A` option enables multiple advanced scanning techniques in a single command, including:

- Operating System Detection (`-O`)
- Service Version Detection (`-sV`)
- NSE (Nmap Scripting Engine) Default Scripts (`-sC`)
- Traceroute

This provides a broad overview of the target system.

## Observations

The scan revealed:

- Multiple open TCP ports
- HTTP and HTTPS services
- Cloudflare HTTP Proxy
- SSL certificate information
- HTTP server headers
- Estimated operating system
- Device type
- Traceroute information showing the network path

## Key Findings

- The host was online and reachable.
- Multiple services were identified.
- SSL certificate details were successfully enumerated.
- Traceroute identified the network distance.
- OS fingerprinting estimated the target's operating system.

## Skills Practiced

- Advanced Enumeration
- OS Fingerprinting
- Service Enumeration
- SSL Enumeration
- Traceroute Analysis
- Nmap NSE Scripts

## Screenshot

(Add your -A scan screenshot here.)

## Lessons Learned

Aggressive scanning combines several Nmap capabilities into one command, making it useful for quickly gathering detailed information about a target during the reconnaissance phase of a security assessment.
