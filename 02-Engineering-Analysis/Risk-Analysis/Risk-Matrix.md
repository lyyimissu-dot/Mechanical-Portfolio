# Risk Matrix – Stacker Crane System

This risk matrix summarises the main hazards identified in the **HAZOP** study and links them with the **quantitative analysis** (error rates and kinetic energy).

---

## 1. Rating Scales

- **Likelihood (L)**  
  1 – Rare 2 – Unlikely 3 – Possible 4 – Likely 5 – Frequent  

- **Severity (S)**  
  1 – Minor 2 – Moderate 3 – Serious damage 4 – Major injury 5 – Fatality / catastrophic  

- **Risk Level**  
  \( R = L \times S \)  
  - 1–5: Low  
  - 6–10: Medium  
  - 11–25: High

> _Image placeholder – coloured risk matrix grid_  
> `![Risk matrix grid](images/risk_matrix_grid.png)`

---

## 2. Key Risks

| **ID** | **Hazard**                             | **Cause (from HAZOP)**                        | **L** | **S** | **R** | **Risk Level** | **Main Mitigations**                                   |
|--------|----------------------------------------|-----------------------------------------------|------:|------:|------:|----------------|--------------------------------------------------------|
| R1     | Load drop from height                 | Overload; wire-rope failure; unsecured load   | 2    | 5    | 10   | Medium–High    | Overload limiter; NDT inspection; better securing     |
| R2     | Collision with rack (fork too high/low)| Positioning error; encoder / limit fault     | 3    | 4    | 12   | High           | Redundant sensors; slow approach; software travel limits |
| R3     | Misplacement / wrong location         | WMS data error; encoder drift                 | 3    | 3    | 9    | Medium         | Data validation; regular calibration                  |
| R4     | Uncontrolled horizontal motion        | Drive failure; control fault                  | 1    | 5    | 5    | Low–Medium     | Emergency stop circuit; speed limiters                |
| R5     | Personnel in aisle during operation   | Poor access control; missing interlocks       | 2    | 5    | 10   | Medium–High    | Fencing; light curtains; access procedures            |

---

## 3. Link to Quantitative Results

- **R2 & R3 – Positioning risks**  
  - Supported by the **load positioning error analysis** (`Load-Positioning-Error.md`).  
  - Error rate is relatively low but non-zero → justifies **Medium to High** risk rating.

- **R1 & R4 – Motion / energy risks**  
  - Related to the **kinetic energy** result in `Kinetic-Energy-Uncertainty.md`.  
  - Even at normal speed, energy (~39 kJ) is large → high severity if control is lost.

---

## 4. Conclusions

- The **highest-priority risks** are:
  - Fork / position errors (R2)
  - Load drop scenarios (R1)
  - Human presence in the aisle (R5)

- Mitigation should focus on:
  - **Redundant sensing and interlocks**
  - **Clear operating procedures**
  - **Regular inspection and calibration**

> _Image placeholder – final summary figure_  
> `![Risk analysis summary](images/risk_conclusion.png)`

