# Lab 03 - Operating System Detection (-O)

## Objective

Identify the operating system running on the target host.

## Command Used

```bash
sudo nmap -O example.com
```

## What the command does

The `-O` option enables operating system detection. Nmap analyzes responses from the target to estimate the operating system and device type.

## Observations

The scan identified:

- Device Type: WAP (Wireless Access Point)
- Operating System: Linux 2.4.x
- OS Details: Actiontec MI424WR-GEN3I WAP, DD-WRT v24-sp2
- Network Distance: 2 hops

Nmap also displayed a warning that the OS detection results may not be completely reliable because it could not find both open and closed ports.

## Key Findings

- Host was online.
- Device appeared to be a wireless access point.
- Estimated Linux operating system detected.
- Network distance was identified.

## Skills Practiced

- OS Fingerprinting
- Device Identification
- Network Enumeration
- Nmap OS Detection

## Screenshot

(Add your -O scan screenshot here.)

## Lessons Learned

Operating system detection helps security professionals understand what type of device they are assessing. This information can be valuable during asset identification and vulnerability assessments.
