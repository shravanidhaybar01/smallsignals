# Day 16 – Incident 02: Authentication Attack

## Objective
Analyze authentication-related log activity to identify
potential brute-force or credential abuse attacks.

## Indicators observed
- Repeated failed login attempts
- High frequency authentication failures
- Attempts targeting a single user account
- Possible successful login after multiple failures

## Log sources reviewed
- /var/log/auth.log
- /var/log/syslog

## Investigation commands

### Failed login attempts
grep "Failed password" /var/log/auth.log

### Successful logins
grep "Accepted password" /var/log/auth.log

### SSH-related activity
grep "ssh" /var/log/auth.log

### Recent authentication events
tail -n 50 /var/log/auth.log

## Assessment
The observed patterns are consistent with
a brute-force or credential stuffing attempt.

## Recommended mitigations
- Enforce strong password policies
- Enable account lockout after failures
- Implement multi-factor authentication (MFA)
- Monitor repeated authentication failures

## Learning outcome
- Understood how authentication attacks appear in logs
- Practiced identifying brute-force indicators
- Improved incident analysis documentation skills
