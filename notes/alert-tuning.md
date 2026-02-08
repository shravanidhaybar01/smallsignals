# Alert Tuning (Beginner Notes)

Alert tuning is the process of improving detection rules
to reduce false positives while still catching real attacks.

## Why alert tuning is needed
- Initial detection rules are often too noisy
- User behavior changes over time
- Attack patterns evolve

## Common tuning methods
- Increasing or decreasing thresholds
- Adding time-based conditions
- Adding context such as user role or location

## Example
Instead of alerting on 3 failed logins,
alert only if there are 10 failed logins
within 5 minutes from the same IP.

## Why tuning matters in SOC
Poorly tuned alerts create alert fatigue
and reduce analyst efficiency.

## My understanding
Alert tuning helps SOC teams focus on
high-quality and meaningful alerts.
