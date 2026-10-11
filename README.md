Apriori Association Rule Mining for Industrial ECE Fault Analysis

## Project Overview
This project implements the  **"Apriori Algorithm" **to discover co-occurring hardware fault patterns in power electronics and embedded system telemetry logs. Instead of standard retail transaction data, this implementation analyzes diagnostic event logs containing faults such as `Overcurrent_Trip`, `High_MOSFET_Temp`, `Voltage_Sag`, and `Gate_Driver_Fault`.

## Problem Statement Parameters
Minimum Support Threshold: 40% (`0.40`)
Minimum Confidence Threshold: 60% (`0.60`)
Evaluated Metrics: Support, Confidence, and Lift

## Key Results & Fault Interpretations
Deterministic Fault Chain (`Confidence = 100%`)**: Whenever `Voltage_Sag` and `High_MOSFET_Temp` occur concurrently, an `Overcurrent_Trip` is guaranteed to follow (`Lift = 1.43`).
Root-Cause Linkage (`Confidence = 100%`)**: `Gate_Driver_Fault` directly predicts thermal stress in `High_MOSFET_Temp` (`Lift = 1.25`).

## Visualization
apriori-fault-analysis/assets/apriori_metrics_plot.png

