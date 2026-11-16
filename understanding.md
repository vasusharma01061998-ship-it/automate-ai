# A-06: 5G Slice SLA Assurance - Understanding

## 1. Understanding
To check the SLA of a 5G Slice. Customer is promised Latency < 20ms, Throughput > 100 Mbps, Availability > 99.9%.
Every 5-min window will be checked if the slice is healthy or anomalous.
If it is degraded, we will tell whether the problem is in Radio, Transport or Core - with proof.
Final decision will be taken by Human, we will only give a Brief + Suggestion.

## What We Will NOT Do
- We will not change slice config
- We will not reserve capacity
- We will not call missing data a breach
- We will not treat correlation as cause

## 2. Token ID
Token ID: tok_A06_demo_001
Format: tok_ + A06_ + demo_001
Work: To identify the system sending telemetry. Secret value will never be shown in logs, only Token ID will be shown.
If it is wrong: REJECT: Invalid Token ID

## 3. Evaluation
We will create 100 synthetic cases. Train on 80, test on 20 held-out cases.
Sources: 3GPP TS 28.552, TS 32.425
