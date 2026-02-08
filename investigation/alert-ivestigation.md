# Alert Investigation (Beginner Notes)

Alert investigation is the process of analyzing
a security alert to determine whether it represents
a real threat or a false positive.

## What analysts check during investigation
- Alert details and reason for trigger
- Source IP address
- User account involved
- Time and frequency of events
- Related log entries

## Basic investigation questions
- Is this activity normal for the user?
- Has this happened before?
- Does the pattern match a known attack?

## Example
If an alert shows multiple failed logins,
an analyst checks:
- Was the user active at that time?
- Did a successful login follow?
- Is the IP known or suspicious?

## Possible investigation outcomes
- False positive
- Suspicious activity
- Confirmed security incident

## My understanding
Investigation helps analysts decide
whether an alert needs further action.
