---
name: s2s-forecasting-expert
description: Expert guidance for AI-based Subseasonal-to-Seasonal (S2S) forecasting systems including FuXi, FengWu, and AIFS with CRPS-based probabilistic verification.
metadata:
  clawdbot:
    emoji: "🌍"
    requires:
      env: []
    files: []
---

# Subseasonal-to-Seasonal (S2S) Forecasting Expert

An expert advisory skill specializing in AI-driven **Subseasonal-to-Seasonal (2–60 day and seasonal-scale) forecasting systems**, including:

- FuXi S2S
- FengWu
- AIFS (AI Forecasting System)
- CRPS-based probabilistic models
- Transformer-based global weather models

This skill provides architectural, training, evaluation, and deployment guidance for modern AI weather systems.

---

## Capabilities

### Architecture Design
- Spatiotemporal transformers for global grids
- Multi-variable atmospheric modeling (Z500, T2M, winds, SST)
- Multi-lead-time output heads
- Ensemble neural forecasting
- Graph-based atmospheric representations

### Training Pipelines
- ERA5-based training workflows
- Hindcast dataset construction
- Rolling lead-time supervision
- Seasonal embeddings
- Atmospheric variable normalization

### Probabilistic Forecasting
- CRPS loss implementation
- Quantile regression outputs
- Ensemble spread calibration
- Reliability diagram interpretation

### Evaluation & Verification
- Continuous Ranked Probability Score (CRPS)
- Anomaly Correlation Coefficient (ACC)
- RMSE across lead times
- Skill vs climatology benchmarks
- Extreme event scoring (Brier score)

### Deployment & Optimization
- Multi-GPU training (FSDP / ZeRO)
- Mixed precision (bfloat16)
- Memory-efficient inference
- Operational forecast pipelines

---

## Example Prompts

- “Design a FuXi-style transformer for 30-day Z500 forecasts.”
- “Implement CRPS loss for probabilistic S2S outputs.”
- “Compare FengWu and AIFS architectures.”
- “Optimize 45-day global forecast inference.”

---

# External Endpoints

This skill does not call any external APIs.

| Endpoint | Purpose | Data Sent |
|----------|---------|-----------|
| None     | N/A     | None      |

---

# Security & Privacy

- No external API calls
- No environment variables required
- No local file access
- No data leaves the system
- Advisory-only functionality

---

# Model Invocation Note

This skill may be automatically invoked when queries relate to:

- Subseasonal-to-Seasonal forecasting
- FuXi, FengWu, or AIFS
- CRPS evaluation
- AI-based weather modeling

Users may opt out by disabling the skill.

---

# Trust Statement

By using this skill, you acknowledge that it provides advisory guidance for AI-based climate and weather forecasting systems. No data is transmitted externally.

---

# Version

v1.0.0  
Last updated: Feb 16, 2026
