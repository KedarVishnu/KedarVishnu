# IS 456 & IS 13920 Compliant RCC Design Suite

![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)
![Framework](https://img.shields.io/badge/GUI-Tkinter-orange.svg)
![Standard](https://img.shields.io/badge/Code-IS%20456%3A2000-green.svg)
![Seismic Standard](https://img.shields.io/badge/Ductile%20Detailing-IS%2013920%3A2016-red.svg)

---

## 📌 Overview

The **RCC Design Suite** is a desktop application built with Python and Tkinter, designed to automate structural concrete element design in accordance with Indian Standard codes (**IS 456:2000** and **IS 13920:2016**). Developed by a senior structural engineer with **38+ years of civil and structural engineering experience**, the suite bridges traditional engineering intuition with modern desktop software automation, high-precision loading diagrams, automated technical reports, and CAD DXF schedule generation.

---

## 🖥️ Application GUI Preview

### 1. Main Interface & Input Overview
![Page 1](./docs/gui_preview/png_images/page_1.png)

---

### 2. One Way & Two Way Slab App GUI
![Page 2](./docs/gui_preview/png_images/page_2.png)

---

### 3. Stair Slab & Beam Design App GUI
![Page 3](./docs/gui_preview/png_images/page_3.png)

---

### 4. Beam & Column Design App GUI
![Page 4](./docs/gui_preview/png_images/page_4.png)

---

### 5. Isolated Footing Design App GUI
![Page 5](./docs/gui_preview/png_images/page_5.png)

---
## 📊 Reports & Output Documentation

### 📑 Technical Report (8 Pages)
<details>
  <summary>🔍 <b>Click to expand Technical Report (Pages 1–8)</b></summary>
  <br>
  
  ![Technical Report Page 1](./assets/technical_report/page_1.png)
  ![Technical Report Page 2](./assets/technical_report/page_2.png)
  ![Technical Report Page 3](./assets/technical_report/page_3.png)
  ![Technical Report Page 4](./assets/technical_report/page_4.png)
  ![Technical Report Page 5](./assets/technical_report/page_5.png)
  ![Technical Report Page 6](./assets/technical_report/page_6.png)
  ![Technical Report Page 7](./assets/technical_report/page_7.png)
  ![Technical Report Page 8](./assets/technical_report/page_8.png)
</details>

---

### 🏗️ Beam Report (4 Pages)
<details>
  <summary>🔍 <b>Click to expand Beam Report (Pages 1–4)</b></summary>
  <br>
  
  ![Beam Report Page 1](./assets/beam_report/page_1.png)
  ![Beam Report Page 2](./assets/beam_report/page_2.png)
  ![Beam Report Page 3](./assets/beam_report/page_3.png)
  ![Beam Report Page 4](./assets/beam_report/page_4.png)
</details>

---

### 📐 AutoCAD DXF Structural Schedule Output
<details>
  <summary>🔍 <b>Click to expand DXF Schedule Output</b></summary>
  <br>

  ![AutoCAD DXF Schedule](./assets/dxf_schedule/Beam_Schedule.png)
  ![AutoCAD DXF Schedule](./assets/dxf_schedule/Column_Schedule.png)
  
</details>

---

## 📊 Structural Loading Diagrams, BMD, SFD & Column P-M Curves

### 1. Beam Deflection Profile
![Beam Deflection](./docs/load_diagram/Beam_Deflection.png)

---

### 2. Bending Moment (BMD) & Shear Force (SFD) Diagrams
![Beam BMD](./docs/load_diagram/Beam_BMD.png)

---

### 3. Column Axial P-M Interaction Curve
![Column Interaction Curve](./docs/load_diagram/Column_Interaction_Curve.png)

---

### 4. Column Section & Tie Layout
![Column Section Layout](./docs/load_diagram/Column_Section_Layout.png)

---

### 5. Footing Plan & Elevation Diagram
![Footing Diagram](./docs/load_diagram/Footing_Diagram.png)

---

## 📂 Data Documentation & Files

* 📄 [Beam Design Results (JSON)](./docs/Beam_Loads/Beam_Results/Beam_Design_Results.json)
* 📄 [Two-Way Slab Loads (JSON)](./docs/Beam_Loads/Two_Way_Slab_Loads/Two_Way_Slab_Loads.json)

## 📄 Detailed System & Compliance Documentation

* 📖 [Read Full Technical Overview & Live Design Outputs](./docs/About_Suite.md)
* 📜 [Read AI Specialist Cover Letter & Statement of Purpose](./docs/Cover_Letter.md)


---

## 👨‍💼 Author & AI Collaboration Vision


**Er. V. P. Kavathekar**  
*Senior Civil & Structural Engineer | Founder, Kalyani Softwares Pune*  
*38+ Years of Structural Engineering & Site Execution Experience*

> **Domain Expert & AI Trainer Vision:**
>This suite was built by pairing 38+ years of senior structural engineering experience with advanced AI collaboration. Acting as an AI Domain Trainer, I translated complex code standards, limit-state formulas, and engineering intuition into automated, validated software logic.
---

## ✨ Core Features & Developed Modules

- **Automated Structural Limit-State Design (IS 456:2000)**: Complete automated limit state design (Ultimate & Serviceability) for RCC structural members:
  - **Flexural & Moment Capacity ($M_u$)**: Automated calculation of ultimate moment of resistance ($M_{u,lim}$), singly/doubly reinforced section sizing, tension ($A_{st}$) and compression ($A_{sc}$) steel areas.
  - **Shear & Torsional Resistance**: Computation of nominal shear stress ($\tau_v$), design shear strength of concrete ($\tau_c, \tau_{c,max}$), and minimum/required vertical stirrup spacing under combined shear and torsion.
  - **Development Length ($L_d$) & Anchorage**: Precise stress transfer length determinations, lap splice detailing, standard $90^\circ/180^\circ$ bend anchorage, and tension/compression bar termination points per Clause 26.2.
  - **Serviceability Checks (Deflection & Cracking)**: Verification of basic span-to-effective-depth ratios ($L/d$) modified by tension ($F_1$) and compression ($F_2$) steel factors per Clause 23.2.1 to prevent excessive long-term sag and flexural cracking.
  - **Slenderness & Lateral Stability**: Slenderness ratio limits ($l_{ef}/b$ and $l_{ef}/d$), lateral support spacing for slender beams (Clause 23.3), and evaluation of secondary P-$\Delta$ bending effects.

- **Ductile Detailing Compliance**: Integrated seismic checks fully compliant with **IS 13920:2016** for high seismic risk zones.
- **Interactive Tkinter Interface**: Desktop GUI providing input validation, step-by-step design calculation stages, and instant design output updates.
- **High-DPI Dynamic Loading Diagrams**: Programmatic generation of 2D load transfer diagrams using **Matplotlib** with continuous/discontinuous edge styles and UDL/trapezoidal load envelopes.
- **Automated Engineering Exports**: Export complete calculation booklets to Word (`.docx`) /and structural schedules to AutoCAD DXF files.
- **Hardware-Bound Protection Engine**: Hardware USB WMI physical serial validation and clock anti-tampering algorithms with AES-GCM encrypted local state tracking.

> 🔒 **Intellectual Property Protection Notice**:  
> To protect core proprietary software intellectual property, the source code of the RCC Design Suite is **not** included in this public repository. This repository serves exclusively as a digital portfolio, technical overview, output validation report archive, and visual feature demonstration.

---

### 📦 Developed Structural Design Modules

| Module Name | Standard Compliance | Primary Engineering Capabilities |
| :--- | :--- | :--- |
| **Beam Design Module** | IS 456:2000 & IS 13920:2016 |Can be used to analyse the beam and can be used to design the beam for given B.M and S.F. and torsion also. Flexural design (singly & doubly reinforced & Flanged Beams), shear design, crack width checks, development length ($L_d$), and ductile detailing. |
| **One-Way Slab Module** | IS 456:2000 (Clause 22, 24) | Staged 3-step workflow for 4 support conditions, programmatic load transfer to supporting beams ($B_1 - B_4$), 2D Matplotlib diagrams, Word report & DXF export. |
| **Two-Way Slab Module** | IS 456:2000 (Table 26) | Table 26 bending moment coefficients for 10 boundary conditions, trapezoidal ($B_1, B_2$) & triangular ($B_3, B_4$) load envelopes, shear load distribution. |
| **Column Design Module** | IS 456:2000 & IS 13920:2016 | P-M interaction curves, axial compression + biaxial bending, slenderness checks ($l_{ex}/D, l_{ey}/b$), ties & ductile reinforcement. |
| **Footing Design Module** | IS 456:2000 (Clause 34) | Isolated footing designs, concentric/eccentric soil pressure distribution, 1-way shear, 2-way punching shear, and flexural steel design. |
| **Staircase Design Module** | IS 456:2000 (Clause 33) | Waist slab thickness, flight loading, riser hight calculation, moment capacity, and rebar scheduling. |
| **For all modules** | Load data transfer in json format & design data save in json format. dxf schedules. Detail docx reports. Government and local body forms.Technical reports for proof checking

---

## 🖼️ Visual Proof & Application Preview

> *This section provides visual verification of the operational Tkinter GUI, dynamic Matplotlib load transfer diagrams, and export capabilities.*

### 1. Tkinter Graphical User Interface
![Tkinter GUI - One-Way Slab Design Interface](./docs/load_diagram/One_Way_Beam_Loads_Diagram.png)
*Figure 1: Interactive Tkinter GUI displaying input forms, boundary conditions, and design parameter controls.*

### 2. 2D Matplotlib Dynamic Load Transfer Diagram
![Matplotlib Beam Load Transfer Envelope](./docs/load_diagram/Two_Way_Beam_Loads_Diagram.png)
*Figure 2: Automatically calculated beam loading diagram showing edge condition styling and UDL/trapezoidal load envelopes.*

### 3. Automated Word Technical Design Report
![Word Technical Design Calculation Report](./assets/technical_report/page_1.png)
*Figure 3: Sample formatted engineering report (.docx) generated automatically by the RCC Design Suite.*

---

## 🛠️ Step-by-Step Guide: How to Add Your Own Screenshots

To add your own GUI screenshots and report images to this README:

1. **Capture Screenshots**:
   - Use Windows Snipping Tool (`Win + Shift + S`) to capture your Tkinter interface, Matplotlib diagrams, or report output.
2. **Create a `docs/` & `assets/` Folder**:
   - Save your GUI previews inside `docs/gui_preview/png_images/` and report exports inside `assets/`.
3. **Push to GitHub**:
   - When you upload to GitHub, all images and diagrams will render automatically!

---

## 📩 Contact & Collaboration

For technical inquiries, software demonstration requests, or AI training collaboration:

- **Author**: Er. V. P. Kavathekar
- **Organization**: Kalyani Softwares Pune
- **Specialization**: RCC Structural Design Automation & IS Code Compliance Verification
- **Email**: `kedar.kavathekar@gmail.com`
- **LinkedIn / Portfolio**: [LinkedIn Profile](https://www.linkedin.com/in/er-vishnu-padmakar-kavathekar-0b826520)

---
*Copyright © 2026 Er. V. P. Kavathekar | Kalyani Softwares Pune. All Rights Reserved.*
