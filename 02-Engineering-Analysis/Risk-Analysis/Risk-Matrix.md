# 📊 Risk Matrix Definition and Classification

## 1. Purpose of the Risk Matrix
This risk matrix is used to **systematically evaluate and classify hazards** identified in the stacker crane system by combining:

- **Severity of consequence**
- **Likelihood of occurrence**

The matrix supports decision-making for:
- Design improvement prioritization  
- Safety mitigation strategy selection  
- Engineering risk communication  

---

## 2. Severity Classification Criteria
Severity is evaluated based on **human safety**, **equipment damage**, and **system downtime**.

| Severity Level | Human Health Impact | Equipment / Cargo Damage | System Impact | Severity Category | Safety Severity Level |
|---|---|---|---|---|---|
| **4** | Fatality or severe injury | Major mast / fork failure | Downtime > 7 days | **Catastrophic** | **4 (TMEF ≈ 1×10⁻⁶)** |
| **3** | Major injury | Gear motor failure | Downtime 2–7 days | **Very Serious** | **3 (TMEF ≈ 1×10⁻⁵)** |
| **2** | Minor injury | Fork deformation; load drop | Downtime 1–2 days | **Serious** | **2 (TMEF ≈ 1×10⁻⁴)** |
| **1** | No injury | Small collision | Downtime < 1 day | **Minor** | **1 (TMEF ≈ 1×10⁻³)** |

> **Note:**  
> TMEF = *Typical Mean Event Frequency*, used here as a reference scale for severity ranking.

---

## 3. Likelihood Classification
The probability of occurrence is categorized into four qualitative levels:

| Likelihood Level | Description |
|---|---|
| **4** | Likely |
| **5** | Unlikely |
| **6** | Improbable |
| **7** | Improbable but not impossible |

---

## 4. Risk Matrix
The overall risk level is determined by intersecting **severity** and **likelihood**.

| Severity ↓ / Likelihood → | **4 Likely** | **5 Unlikely** | **6 Improbable** | **7 Improbable but not impossible** |
|---|---|---|---|---|
| **4 Catastrophic** | **A** | **A** | **B** | **C** |
| **3 Very Serious** | **A** | **B** | **C** | **D** |
| **2 Serious** | **B** | **C** | **D** | Negligible |
| **1 Minor** | **C** | **D** | Negligible | Negligible |

---

## 5. Risk Level Interpretation

| Risk Level | Interpretation | Required Action |
|---|---|---|
| **A** | Unacceptable risk | Immediate design change required |
| **B** | High risk | Mitigation measures mandatory |
| **C** | Moderate risk | Monitoring and design review |
| **D** | Low risk | Acceptable with standard controls |
| **Negligible** | Minimal risk | No action required |

---

## 6. Figures (Insert Later)

### 6.1 Risk Matrix Image
> *(Insert visual risk matrix image here)*

```md
![Risk Matrix Overview](images/risk-matrix.png)
