# 🔧 AOI333 Standard Cell Design (65nm CMOS)

## 📌 Overview
This project involves the **design, layout, and characterization of an AOI333 (AND-OR-Invert) standard cell** in 65nm CMOS technology.

Both **complex and non-complex implementations** were analyzed and compared in terms of **delay, power, and robustness across PVT corners**.

---

## 🧠 Logic Function

F = ¬((A·B·C) + (D·E·F) + (G·H·I))

---

## ⚙️ Design Flow
- Transistor-level schematic design (Virtuoso & Xcircuit)
- Transistor sizing optimization  
- Stick diagram and layout design  
- DRC & LVS verification  
- Pre-layout and post-layout simulation  
- PVT corner analysis  

---

## 🛠️ Tools Used
- Cadence Virtuoso (Schematic + Layout)
- Mentor Calibre (DRC & LVS)
- Eldo SPICE (Simulation)

---

## 📐 Design Details
- Technology Node: **65nm**
- Total MOSFETs: **18**
- Layout Area: **~10.78 µm²**
- Track Count: **13**

### Transistor Sizing:
- PMOS: W = 0.45 µm, L = 0.06 µm  
- NMOS: W = 0.225 µm, L = 0.06 µm  

---

## 📊 Performance Analysis

### ⏱️ Delay (Post-Layout, SS Corner)
- Fall Propagation Delay: **~2.08 ns**
- Rise Propagation Delay: **~2.06 ns**

### ⚡ Dynamic Power (Post-Layout)
- TT (1.2V, 25°C): **~1.25 mW**
- FF (1.32V, -40°C): **~2.25 mW**
- SS (1.08V, 125°C): **~1.71 mW**

### 🔋 Static Power (Post-Layout)
- Ranges from **pW to hundreds of pW** depending on PVT corner

---

## 🔬 Key Observations
- Post-layout delays increased due to **parasitic capacitances**
- Complex gate implementation showed **better delay performance** compared to non-complex design
- Power consumption increases significantly at higher voltage (FF corner)
- PVT variation has strong impact on timing and leakage

---

## 🔄 Complex vs Non-Complex Design

| Metric | Complex Gate | Non-Complex Gate |
|-------|-------------|------------------|
| Delay | Lower | Higher |
| Power | Moderate | Higher |
| Area | Optimized | Larger |

👉 Complex implementation is more efficient for high-performance designs

---

## 🚀 Highlights
- Full **standard cell design flow (schematic → layout → verification)**
- Detailed **PVT-based characterization**
- Comparison of **design styles (complex vs non-complex)**
- Real **post-layout simulation data included**

---

## 📄 Documentation
👉 [View Full Presentation](AOI333_Design_Presentation.pdf)

---

## 🧠 Learnings
- Impact of **layout parasitics on delay**
- Trade-offs between **area, power, and speed**
- Importance of **PVT analysis in standard cell design**
- CMOS logic optimization techniques

---

## 🔮 Future Work
- Standard cell characterization (timing libraries)
- Integration into synthesis flow
- Power optimization techniques
- Extension to full cell library

---

## 👨‍💻 Author
**Aman Kumar**  
B.Tech ECE (VLSI), IIIT Delhi  

🔗 GitHub: https://github.com/aman22060  
🔗 LinkedIn: https://www.linkedin.com/in/amankumar0679/
