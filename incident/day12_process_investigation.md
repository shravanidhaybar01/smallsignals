# Day 12 – Linux Process Investigation Basics

## Why this matters
In cybersecurity and SOC roles, identifying suspicious processes is a core skill.
Attackers often leave traces through unusual running processes.

## Common commands to investigate processes

### View all running processes
ps aux

### Real-time process monitoring
top

### Better interactive monitoring
htop

## What makes a process suspicious?
- Unusual or random names
- High CPU or memory usage
- Running as root unnecessarily
- Commands like:
  - bash -i
  - nc / netcat
  - python -c
  - suspicious background scripts

## Analyst mindset
Do not panic.
Observe → Compare → Validate → Report.

## Learning outcome
Today I learned how to:
- List running processes
- Identify abnormal behavior
- Think like a SOC analyst during incident response
