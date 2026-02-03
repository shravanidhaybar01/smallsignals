# Day 15 – Incident Timeline Basics

## What is an incident timeline?
An incident timeline is a chronological record of events
that helps security analysts understand:
- What happened
- When it happened
- How the system was compromised

## Why timelines matter in cybersecurity
Without a timeline, incident response becomes guesswork.
Timelines help identify root cause and prevent future attacks.

## Basic incident timeline structure

1. Initial access
   - Phishing, weak credentials, exposed services

2. Execution
   - Suspicious process started
   - Unauthorized scripts or binaries executed

3. Persistence
   - Backdoors, cron jobs, startup scripts

4. Command & Control
   - Outbound network connections to attacker systems

5. Detection
   - Logs, alerts, abnormal system behavior

## Sources used to build a timeline
- Authentication logs (/var/log/auth.log)
- System logs (/var/log/syslog)
- Running processes (ps, top)
- Network connections (ss, netstat)

## SOC analyst mindset
Correlate logs + processes + network data.
Do not assume — verify.

## Learning outcome
Today I learned:
- How incident timelines are structured
- How analysts correlate multiple data sources
- How to think systematically during investigations
