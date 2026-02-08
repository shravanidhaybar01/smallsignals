# Day 14 – Network Connections Basics (Linux)

## Why network monitoring matters
Attackers often maintain access through network connections.
Understanding active connections helps detect reverse shells,
malware communication, and data exfiltration.

## Important commands for network analysis

### View active connections
netstat -tunlp

### Modern alternative to netstat
ss -tunlp

### Check listening ports
ss -lntp

### Show open files with network connections
lsof -i

## What to look for in suspicious activity
- Unknown services listening on ports
- High-numbered ports unexpectedly open
- External IP addresses communicating frequently
- Services running as root without reason

## Example suspicious signs
- Port 4444 or 1337 listening
- Outbound connections to unknown IPs
- Background processes maintaining connections

## SOC analyst workflow
Identify connections → Map process → Validate service → Take action

## Learning outcome
Today I learned:
- How to view active network connections
- How to identify abnormal ports and traffic
- How SOC analysts detect network-based threats
