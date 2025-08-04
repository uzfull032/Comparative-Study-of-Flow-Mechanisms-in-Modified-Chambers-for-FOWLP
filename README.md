# 🌀 Comparative Study of Flow Mechanisms in Modified FOWLP Chambers

This repository provides a summary of a CFD simulation study analyzing the flow mechanisms in modified soft bake chambers used in the Fan-Out Wafer-Level Packaging (FOWLP) process.

---

## 🔬 Abstract

This study investigates flow characteristics in the FOWLP soft bake process using CFD simulations with various inlet shapes (hole, slit, plain) and the presence or absence of baffles. A realizable k–ε turbulence model with Enhanced Wall Treatment was applied in ANSYS Fluent. Ring-type inlets showed strong influence in baffle-free configurations, whereas baffle structures contributed to improved pressure uniformity (99.87–99.90 kPa) and minimal standard deviations (<0.01 kPa). This suggests that ring inlets and baffle design are crucial for flow stability in thermal processing.

---

## 📐 Mathematical Model
The realizable k–ε turbulence model with Enhanced Wall Treatment (EWT) was used to simulate turbulent flow inside the chamber. The governing equations for the turbulent kinetic energy 𝑘 and the dissipation rate 𝜀 are as follows:
- **Model**: Realizable *k–ε* with Enhanced Wall Treatment (EWT)
  <p align="left"><img width="682" height="288" alt="image" src="https://github.com/user-attachments/assets/ad540034-7f1c-4610-8f99-72323b329936" />
  <p align="left"><img width="694" height="368" alt="image" src="https://github.com/user-attachments/assets/27fcb960-5620-426a-be97-77ba819547fa" />

- **Boundary Conditions**:
  - Modified overall structure:
  <p align="left"><img width="800" height="264" alt="image" src="https://github.com/user-attachments/assets/70878ec3-44d7-476e-8e84-d55edb4dba80" />
  
  - Inlet pressure: 100 kPa
  - Outlet pressure: 0.05 kPa or 0.15 kPa
  - 30°–90° periodic symmetry applied

   <p align="left"><img width="321" height="255" alt="image" src="https://github.com/user-attachments/assets/3761ff0a-4e7e-4ee7-a233-2737af11ce9d" />

---

## 📊 Key Findings

| Inlet Type | Baffle | Avg Pressure (kPa) | Pressure STD (kPa) | Flow Behavior |
|------------|--------|--------------------|---------------------|----------------|
| Hole       | ❌     | ~98.9              | up to 0.4           | High speed center, unstable |
| Slit       | ❌     | ~99.0              | ~0.1                | Gradual gradient, mid-stable |
| Plain      | ❌     | ~98.9              | ~0.06               | Similar to hole |
| Hole       | ✅     | 99.89              | ~0.00001            | Very stable |
| Slit       | ✅     | 99.90              | ~0.002              | Uniform, slight edge loss |
| Plain      | ✅     | 99.87              | ~0.013              | Smooth, very stable |

- Baffle structures induced flow stagnation and enhanced uniformity.
- Ring-type inlets dominated flow without baffles.
- All baffle cases showed pressure differences < 0.03 kPa.

---

## ✅ Conclusion

The combination of **ring-shaped inlets** and **baffle structures** is highly effective in achieving pressure uniformity and suppressing turbulent fluctuations on the wafer surface during the soft bake process. These findings offer practical design guidelines for FOWLP chamber optimization. Future work should include experimental validation.
