# AI Programming Methodology Comparison: PC-CIP vs Traditional Approaches

## Overview
This document compares **Prompt-Centric Causal Invariant Programming (PC-CIP)** with traditional programming methodologies, focusing on **AI-driven and prompt-based development**.

---

## Methodology Comparison

| Dimension | PC-CIP (AI Programming Methodology) | OOP / FP / Clean Architecture |
|--------|-------------------------------------|--------------------------------|
| Primary author | AI (LLM) | Human |
| Source of truth | Prompt + invariants | Code |
| Change handling | Invariant-preserving diffs | Refactor-heavy |
| Failure modeling | Mandatory | Often implicit |
| Side effects | Explicitly constrained | Often implicit |
| Auditing | Built-in proof pack | Manual |
| Prompt suitability | Native | Poor |
| Hallucination resistance | High | Low |
| Evolution over time | Stable | Fragile under churn |

---

## Key Insight
Traditional methodologies optimize **how humans think**.  
PC-CIP optimizes **how AI systems reason**.

