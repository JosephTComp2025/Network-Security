# Wazuh Brute Force Detection Parser

## Context
Hydra brute force attack simulated against Ubuntu SSH.
Wazuh manager detected failed login attempts in `alerts.log`.

## Python Automation
This script parses Wazuh alerts and summarizes failed SSH attempts by source IP.

Demonstrates SOC workflow: attack → detection → automation.
Shows Python applied to log triage.
