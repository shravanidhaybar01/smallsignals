# Day 13 – Log Analysis Basics (Linux)

## Why log analysis is important
Logs are the first place a SOC analyst looks during an incident.
They record authentication attempts, system errors, and suspicious activity.

## Important Linux log files

### Authentication logs
/var/log/auth.log

Contains:
- Login attempts
- sudo usage
- SSH activity

### System logs
/var/log/syslog

Contains:
- System events
- Service status
- Errors and warnings

## Useful commands for log analysis

### View entire log
cat /var/log/auth.log

### View logs page by page
less /var/log/auth.log

### Search for keywords
grep "failed" /var/log/auth.log
grep "ssh" /var/log/auth.log

### View last entries
tail -n 20 /var/log/auth.log

## What looks suspicious in logs?
- Multiple failed login attempts
- Logins at odd hours
- Repeated sudo failures
- Unknown IP addresses

## SOC analyst approach
Collect logs → Filter data → Identify patterns → Escalate findings

## Learning outcome
Today I learned:
- Where Linux logs are stored
- How to read and search logs
- How SOC analysts detect suspicious behavior
