# Kinetic Energy Uncertainty Analysis

## 1. Purpose and Background

During high-speed horizontal travel of a stacker crane, especially under emergency stop conditions, the kinetic energy of the moving system must be safely dissipated by structural components and braking mechanisms.

However, uncertainties in system mass, velocity, and stopping distance may lead to deviations between expected and actual kinetic energy levels. This analysis evaluates how such uncertainties influence safety risk and structural demand.

This study is intended as a **risk-oriented engineering assessment**, not a detailed transient dynamic simulation.

---

## 2. Definition of Kinetic Energy

The kinetic energy of the moving stacker crane system is defined by the classical mechanical relationship between mass and velocity.

![Kinetic Energy Formula](images/ke_formula.png)
<!-- TODO: Insert kinetic energy formula image here
     Suggested content: KE = 1/2 · m · v²
     Filename: ke_formula.png -->

Where:

- **m** = effective moving mass of the crane system  
- **v** = horizontal travel velocity  

The effective mass includes the crane frame, carriage, payload, and a portion of rotating components converted into equivalent translational mass.

---

## 3. Sources of Uncertainty

Several uncertainty sources may affect the actual kinetic energy during operation:

### 3.1 Mass Uncertainty

- Payload weight variation  
- Optional attachments or tooling  
- Manufacturing tolerances  

![Mass Uncertainty Illustration](images/mass_uncertainty.png)
<!-- TODO: Insert mass uncertainty illustration or schematic -->

---

### 3.2 Velocity Uncertainty

- Control system overshoot  
- Encoder resolution limits  
- Emergency stop reaction delay  

![Velocity Uncertainty Illustration](images/velocity_uncertainty.png)
<!-- TODO: Insert velocity uncertainty illustration -->

---

### 3.3 Stopping Distance Uncertainty

- Brake performance degradation  
- Rail-wheel friction variation  
- Structural flexibility  

![Stopping Distance Illustration](images/stopping_distance_uncertainty.png)
<!-- TODO: Insert stopping distance or braking distance illustration -->

---

## 4. Uncertainty Propagation Concept

The combined effect of mass and velocity uncertainty leads to a range of possible kinetic energy values rather than a single deterministic value.

Instead of a closed-form equation, this analysis considers **upper-bound and lower-bound scenarios**:

- Minimum kinetic energy (light load + nominal speed)  
- Nominal kinetic energy  
- Maximum kinetic energy (heavy load + speed overshoot)

![Kinetic Energy Range Diagram](images/ke_uncertainty_range.png)
<!-- TODO: Insert kinetic energy range diagram -->

---

## 5. Worst-Case Energy Scenario

The worst-case kinetic energy occurs when:

- Payload mass is at maximum allowable value  
- Travel speed exceeds nominal due to control delay  
- Emergency stop occurs at peak velocity  

![Worst Case Scenario Diagram](images/worst_case_ke.png)
<!-- TODO: Insert worst-case kinetic energy scenario illustration -->

This scenario governs structural checks and safety margin evaluation.

---

## 6. Engineering Implications

Elevated kinetic energy directly increases:

- Structural bending demand on columns and base frame  
- Contact forces at wheel–rail interfaces  
- Stress concentration at joint and connection regions  

![Structural Impact Illustration](images/structural_impact.png)
<!-- TODO: Insert structural impact or stress illustration -->

---

## 7. Risk Interpretation

Rather than relying on absolute kinetic energy values, this analysis focuses on **risk classification**:

- Likelihood of exceeding design energy absorption capacity  
- Severity of potential structural or system damage  
- Relationship to emergency stop frequency  

This information feeds directly into the **Risk Matrix and HAZOP analysis**.

---

## 8. Limitations

- Linear static assumptions  
- No explicit transient dynamic response  
- No thermal effects from braking energy dissipation  

These limitations are acceptable for **early-stage risk screening** and portfolio demonstration purposes.

---

## 9. Conclusion

Kinetic energy uncertainty represents a critical contributor to stacker crane operational risk. By evaluating conservative upper-bound scenarios, the analysis ensures that structural and safety-related design decisions remain robust against real-world variability.

This approach supports risk-informed engineering decisions prior to detailed dynamic simulation or physical testing.
