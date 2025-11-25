# 🛠️ Mechanical Module — leg-aid-exo

The Mechanical module contains all CAD models, 3D-printable components, structural elements, and assembly resources used to build the leg-aid-exo lower-limb exoskeleton.  
This subsystem is responsible for the physical frame, user-interface components, and load-transmission elements.

---

## 📁 Contents

- **3d_print_files/**  
  STL/STEP files for printed components (cuffs, brackets, housings).

- **machined_parts/**  
  Aluminum and carbon-fiber parts requiring CNC or manual machining.

- **carbon_fiber/**  
  Uprights, motor mounts, and structural plates.

- **cuffs/**  
  Adjustable thigh cuff designs, padding guides, and sizing options.

- **assembly/**  
  Exploded views, mechanical drawings, and step-by-step build instructions.

---

## 🧩 Mechanical Overview

The leg-aid-exo mechanical system is designed to be:

- **Lightweight** → made from carbon fiber, nylon composites, and minimal hardware  
- **Modular** → all components can be adapted for different users and experiments  
- **Open-source** → fully documented and customizable  
- **Compatible** → integrates directly with the OpenExo actuation and belt architecture  

The system supports lower-limb assistance through a hip-mounted motor interface connected to a thigh cuff using a reinforced upright.

---

## 🔧 Manufacturing Notes

- Cuffs and brackets: **3D printed (Nylon, Onyx, PETG)**  
- Uprights and high-load parts: **Carbon fiber or aluminum**  
- Hardware: Metric fasteners (M5/M6 recommended for load-bearing points)

---

## 📚 Documentation

Full build instructions and diagrams can be found in:

- `docs/build_guide.pdf`  
- `docs/assembly_instructions.md`  

These guides include sizing, fit adjustments, and calibration notes for mechanical alignment.

---

## 🤝 Contributions

Mechanical improvements, redesigns, and alternative components are welcome.  
Please include CAD source files (.STEP, .SLDPRT, .F3D) when possible.

