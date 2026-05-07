---
name: performance
description: "Profile execution, identify bottlenecks, and optimize resource utilization."
risk: unknown
source: community
date_added: "2026-05-07"
---

# Performance Skill

## When to Use
Use this skill when you need to:
- Identify slow code paths, N+1 queries, or memory leaks.
- Propose algorithmic optimizations or caching strategies.
- Benchmark changes to quantify performance impact.

## Prerequisites
- Access to profiling tools (e.g., `cProfile`, `py-spy`, browser devtools).
- Baseline performance metrics.

## Common commands
- `python -m cProfile script.py`
- `time ./command`

## Notes
- "Trace before you tune": Always back optimization claims with profile data.
- Maintain a balance between performance and readability.

## Limitations
- Optimization may introduce complexity; justify every trade-off.
- Benchmarks in isolated environments may not reflect production load.
