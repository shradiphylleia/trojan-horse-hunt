# trojan-horse-hunt
Trojan Horse Hunt in Time Series Forecasting(ESA)


# Trojan Horse Hunt 

This repository contains a **fully reproducible pipeline**
It adapts the Neural Cleanse method to the multivariate telemetry setting (3 channels × 75 samples)
---

## What this pipeline does
- Loads the pack of **45 poisoned N-HiTS models** released by the organizers  
- For each model:  
  - Probes for potentially poisoned channels  
  - Runs the **λ–α–β adaptive optimization loop** to reconstruct candidate triggers  
  - Visualizes triggers aligned with model forecasts  
- Assembles all recovered triggers into the exact `(45, 75, 3)` submission format 
