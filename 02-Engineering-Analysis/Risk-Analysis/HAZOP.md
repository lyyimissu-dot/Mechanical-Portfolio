# HAZOP Study – Stacker Crane

This document summarises the **HAZOP (Hazard and Operability)** analysis I performed for the stacker-crane system.

> _Image placeholder – HAZOP workflow_  
> `![HAZOP workflow](images/hazop_workflow.png)`

---

## 1. Nodes and Parameters

Analysed nodes:

1. **Cargo node** – pallet and load on the fork
2. **Fork node** – fork vertical / horizontal position relative to rack and pallet

Typical guidewords: **More / Less / No / High / Low / Mis- / Other than**.

---

## 2. HAZOP – Cargo Node

> _Image placeholder – Cargo node sketch_  
> `![Cargo node](images/hazop_cargo_node.png)`

| **Parameter** | **Deviation** | **Possible Causes**                                                | **Consequences**                                                   | **Safeguards / Recommendations**                                      |
|--------------|---------------|--------------------------------------------------------------------|--------------------------------------------------------------------|------------------------------------------------------------------------|
| Load mass    | More          | Overloading; wrong pallet type; sensor calibration drift          | Wire-rope overload; structural damage; potential load drop        | Overload limiter; regular load-cell calibration; clear load-rating labels |
| Load mass    | Less          | Incorrect data in WMS; empty pallet mistakenly treated as loaded  | Inefficient storage; incorrect inventory; unexpected dynamics     | Cross-check with barcode / vision; WMS validation rules               |
| Load secured | No / Poor     | Missing straps; operator negligence; worn pallet condition        | Load shift during acceleration or emergency stop; loss of stability | Visual inspection; interlock requiring “load secured” confirmation     |

---

## 3. HAZOP – Fork Node

> _Image placeholder – Fork node sketch_  
> `![Fork node](images/hazop_fork_node.png)`

| **Parameter**         | **Deviation** | **Possible Causes**                              | **Consequences**                                                   | **Safeguards / Recommendations**                                   |
|-----------------------|---------------|--------------------------------------------------|--------------------------------------------------------------------|--------------------------------------------------------------------|
| Fork height           | Higher        | Limit switch failure; encoder error; wrong target | Collision with upper beam or pallet above; risk of load drop      | Redundant limit switches; software height limits; speed reduction near rack |
| Fork height           | Lower         | Positioning error; deflection not compensated    | Collision with rack beam; fork trapped under pallet                | Height offset compensation; slow approach mode                     |
| Fork lateral position | Left / Right  | Misalignment; wrong reference; installation error | Side collision; recurring misplacement on one side                 | Alignment procedure; mechanical stops; positional verification     |
| Fork tilt / level     | Not level     | Uneven wear; sensor failure; mechanical damage   | Uneven load distribution; increased local stress                   | Level sensor monitoring; preventive maintenance                    |

---

## 4. Key Findings

- **Most critical deviations** involve **overload** and **fork position errors**.
- Many hazards can be mitigated by:
  - Redundant **limit switches / sensors**
  - **Speed reduction** near the rack
  - Clear **load-rating and operating procedures**
- The HAZOP results are later mapped into the **quantitative risk matrix** in `Risk-Matrix.md`.

> _Image placeholder – HAZOP summary chart_  
> `![HAZOP summary](images/hazop_summary.png)`

