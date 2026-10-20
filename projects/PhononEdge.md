# PhononEdge
### Context-aware condition monitoring for rotating equipment

**Status:** Engineering design and competition submission. **Physical prototype and performance validation are pending.**  
**Team:** Three mechanical engineering students.  
**Platform under consideration:** Arduino UNO Q.

---

## The problem

A motor's vibration changes for reasons other than mechanical faults. Rotational speed, temperature, load and sensor conditions can all influence its measurements. A simple fixed threshold can therefore confuse normal operating changes with evidence of a fault.

**Design question:** *Can we evaluate machine behavior in context instead of judging vibration in isolation?*

## Proposed system

The PhononEdge concept combines:

| Signal | Intended role |
| --- | --- |
| Vibration (piezo sensor) | Observe mechanical behavior and changes over time. |
| Rotational speed (Hall sensor) | Interpret vibration relative to operating speed. |
| Temperature (NTC sensor) | Account for changing thermal conditions. |

The proposed workflow is to establish reference behavior, compare new measurements under similar operating conditions and mark sustained deviations for further review.

A design priority is **data quality**: disconnected sensors, unreliable measurements or missing operating context should not produce an unjustifiably confident fault diagnosis.

## Engineering plan

1. Define a controlled rotating-equipment test setup and safe operating limits.
2. Acquire synchronized vibration, speed and temperature data.
3. Characterize reference behavior across selected normal conditions.
4. Introduce controlled, bounded mechanical changes under appropriate safety controls.
5. Evaluate false alarms, missed detections and measurement-quality failures.

These are **planned validation activities**, not reported experimental outcomes.

## Project contribution and lessons

I participated in developing this team project and its competition application. The work involved translating an industrial problem into a proposed sensor architecture, decision logic and test plan.

The project taught me the importance of separating **a convincing technical design** from **performance that has actually been demonstrated**.

## Boundaries

- No claim that hardware validation or field deployment is complete.
- No measured accuracy, detection rate or cost reduction is claimed.
- Results on one motor would not automatically establish general performance across different industrial equipment.

## Longer-term interest

My mechanical engineering background and growing interest in software and security could eventually meet in industrial/OT cybersecurity, where understanding physical processes and safe system behavior is essential.

[← Back to profile](../README.md)
