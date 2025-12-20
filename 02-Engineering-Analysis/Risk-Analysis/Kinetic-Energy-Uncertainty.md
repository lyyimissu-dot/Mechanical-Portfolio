# Kinetic Energy–Based Risk Analysis

## Purpose

This section evaluates the **risk of uncontrolled horizontal motion** in an automated stacker crane using a **kinetic-energy model with uncertainty propagation**.  
The goal is to support **buffer sizing and speed-limit decisions** under worst-case operating conditions.

---

## Kinetic Energy Model

The horizontal kinetic energy of the crane–load system is defined as:

📌 *Insert equation image here*  
`KE = 1/2 · (m_crane + m_load) · v²`

Where:

- `m_crane` = crane self-weight  
- `m_load` = payload mass  
- `v` = horizontal travel speed  

This represents the **maximum energy that must be absorbed** during emergency stop or control failure.

---

## Uncertainty Consideration

Two dominant uncertainty sources are considered:

- Payload mass variation  
- Velocity control error  

Using first-order error propagation, the **upper-bound kinetic energy** is estimated rather than relying on a nominal value.

📌 *Insert uncertainty propagation formula image here*

---

## Engineering Insight

- Nominal kinetic energy defines **baseline buffer requirements**
- Propagated uncertainty defines **design safety margin**
- If upper-bound energy exceeds buffer capacity, **speed reduction or buffer upgrade is required**

This approach links **mechanical modeling** directly to **risk mitigation decisions**.

---

## Role in Overall Risk Assessment

This analysis complements:

- **HAZOP** → identifies uncontrolled motion hazards  
- **Risk Matrix** → classifies severity as high  
- **Error-rate analysis** → reflects operational variability  

Together, they provide a **quantitative justification** for safety-related design choices.
