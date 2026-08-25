 # IS 456 & IS 13920 Compliant RCC Design Suite

An automation and verification suite developed to perform rigorous structural engineering designs and safety checks for Reinforced Concrete Cement (RCC) building elements. The application engine is fully compliant with Indian Standard codes of practice, including **IS 456:2000, IS 875, SP 16 design handbooks, and IS 13920 ductile detailing**.

Built using **Python and Tkinter**, this desktop tool acts as a deterministic validation engine to eliminate structural engineering calculation errors and ensure absolute code compliance.

---

## Core System Features

*   **Beam Design Module (First Principles & Stress-Strain Block)**: Employs exact $C_u = T_u$ equilibrium from first principles, precise rectangular-parabolic stress-strain block parameters, and exact internal lever arm ($z$) calculations for singly reinforced, doubly reinforced, and flanged sections.
*   **Slab Design Module (One-Way & Two-Way IS Coefficients)**: Computes design bending moments and shear forces using IS 456 code coefficients (Tables 12 & Annex D), executing comprehensive flexural checks, minimum reinforcement enforcement, and active serviceability (deflection $L/d$) checks.
*   **Column Design Module (Strain Compatibility & Bresler Contour Method)**: Evaluates axial load and biaxial bending interaction using exact non-linear strain compatibility across section layers and applies the Bresler Load Contour Method $\left(\left(\frac{M_{ux}}{M_{ux1}}\right)^{\alpha_n} + \left(\frac{M_{uy}}{M_{uy1}}\right)^{\alpha_n} \le 1.0\right)$ for rigorous capacity verification.
*   **Footing Design Module (Dual Shear & Critical Section Flexure)**: Executes complete limit state design for isolated/combined footings—calculating maximum bending moment at column faces, one-way (beam) shear at critical section $d$, and two-way (punching) shear stress at the critical perimeter $d/2$.
*   **Active Serviceability Checks**: Calculates non-linear continuous parameters, including steel stress ($f_s$) and deflection modification factor ($F_1$) to enforce span-to-depth constraints per Clause 23.2.1.
*   **Ductile Detailing Compliance**: Built-in verification logic mapping structural requirements to **IS 13920** boundaries (e.g., column confinement zone hoop spacing).
*   **Analytical SP 16 Shear Strength Formulations**: Implements the analytical formulas from the SP 16 handbook for concrete shear strength ($\tau_c$) calculation, eliminating manual Table 19 interpolation and human approximation errors.

---

## Purpose: Bridging Engineering Expertise and AI Safety

*The full source engine of this suite remains private.* However, selected algorithmic modules are showcased here to demonstrate a structural code review mindset. 

### Why I Train AI Models:
As an engineer with **38+ years of field experience**, I recognize that the upcoming generation of young engineers will heavily rely on artificial intelligence tools. If an AI hallucinates a formula or misapplies an IS code factor, the consequences can compromise physical safety. 

My mission in AI training is to turn contract tasks into elite mentoring sessions—sharing deep, battle-tested engineering **knowledge** rather than superficial internet information. I audit AI-generated code to guarantee that tomorrow's digital engineering models are accurate, deterministic, and safe for human infrastructure.

---

## Technology Stack & Requirements

*   **Language**: Python 3.13
*   **GUI Framework**: Tkinter
*   **Libraries**: Standard Math, NumPy (for tabular vector arrays)
*   **Compliance Baseline**: Bureau of Indian Standards (BIS) codes (IS 456, IS 13920, IS 875, SP 16)
