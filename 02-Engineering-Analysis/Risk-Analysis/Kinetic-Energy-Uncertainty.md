# Kinetic Energy Uncertainty Analysis

## 1. Background

During horizontal travel of a stacker crane, especially under emergency stop conditions, the kinetic energy of the moving system must be safely absorbed by the structure and braking system.

Due to uncertainties in payload mass, travel speed, and braking response, the actual kinetic energy may deviate from its nominal value. This analysis evaluates the safety impact of such uncertainty from a risk perspective.

---

## 2. Kinetic Energy Definition

The kinetic energy of the moving system is determined by its effective mass and horizontal velocity.

![Kinetic Energy Formula](images/ke_formula.png)
<!-- TODO: Insert kinetic energy formula image
     Suggested content: KE = 1/2 · m · v² -->

The effective mass includes the crane structure, carriage, payload, and equivalent rotating mass.

---

## 3. Sources of Uncertainty

Key uncertainty sources include:

- **Mass variation** due to payload changes and attachments  
- **Velocity overshoot** caused by control delay during emergency stop  
- **Braking uncertainty** from friction and system response variability  

![Uncertainty Sources Illustration](images/ke_uncertainty_sources.png)
<!-- TODO: Insert uncertainty source illustration -->

These factors lead to a range of possible kinetic energy values rather than a single deterministic value.

---

## 4. Engineering and Risk Implications

The worst-case kinetic energy scenario occurs when maximum payload and speed overshoot coincide during emergency braking.

![Worst Case Kinetic Energy Scenario](images/worst_case_ke.png)
<!-- TODO: Insert worst-case scenario illustration -->

Elevated kinetic energy increases structural demand and contributes to higher risk levels in the system risk matrix. This analysis supports conservative design decisions and feeds into the overall HAZOP and risk assessment framework.
