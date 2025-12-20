# Kinetic Energy & Uncertainty – Emergency Stop Scenario

This document analyses the **kinetic energy** of the stacker crane during horizontal travel and evaluates the **uncertainty** in that energy when an **emergency stop** occurs.

---

## 1. Scenario Description

- Operating mode: **Horizontal travel** along the aisle
- Direction: **+Y** (forward)
- Event: **Emergency stop** from nominal travel speed
- Goal: Estimate **impact severity potential** using kinetic energy.

> _Image placeholder – crane motion sketch_  
> `![Crane motion](images/kinetic_motion_sketch.png)`

---

## 2. Parameters and Assumptions

- Crane self-weight \( M = 10,000 \,\text{kg} \)
- Rated load \( m = 1,000 \pm 5 \,\text{kg} \)
- Maximum travel speed \( v = 160 \pm 2 \,\text{m/min} \)

Converted speed:

\[
v = \frac{160}{60} \approx 2.67 \,\text{m/s}
\]

---

## 3. Kinetic Energy Calculation

\[
E = \frac{(M + m) v^2}{2}
\]

Substituting the nominal values:

\[
E \approx \frac{(10,000 + 1,000) \times 2.67^2}{2} \approx 39.1 \,\text{kJ}
\]

---

## 4. Uncertainty Propagation

Treat \( m \) and \( v \) as independent variables with small uncertainties.

\[
E = \frac{1}{2}(M+m)v^2
\]

\[
\frac{\partial E}{\partial m} = \frac{v^2}{2}
\]

\[
\frac{\partial E}{\partial v} = (M+m)v
\]

Approximate uncertainty in \(E\):

\[
\sigma_E = \sqrt{\left(\frac{\partial E}{\partial m} \sigma_m \right)^2
            + \left(\frac{\partial E}{\partial v} \sigma_v \right)^2}
\]

With:

- \( \sigma_m = 5 \,\text{kg} \)
- \( \sigma_v = 2 \,\text{m/min} = 0.033 \,\text{m/s} \)

The final result is approximately:

\[
E = 39.1 \pm 0.5 \,\text{kJ}
\]

---

## 5. Engineering Interpretation

- Even at moderate warehouse speeds, the **kinetic energy is high** due to the large mass.
- A **controlled deceleration** is essential to avoid:
  - Excessive loads on the mast and rails  
  - Loss of stability if the load is not properly secured
- The small uncertainty band (±0.5 kJ) shows that the energy estimate is **robust** with respect to typical variations in load and speed.

> _Image placeholder – kinetic energy bar chart_  
> `![Kinetic energy with uncertainty](images/kinetic_energy_bar.png)`

> _Image placeholder – equation snapshot from report_  
> `![Error propagation derivation](images/error_propagation.png)`

