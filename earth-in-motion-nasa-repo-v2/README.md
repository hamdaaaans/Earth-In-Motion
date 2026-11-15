# Earth in Motion — NASA Space Apps Challenge 2026

**Challenge:** Dancing with the SARs  
**Live Application:** https://earth-in-motion-nasa.base44.app/  
**License:** MIT

---

## Project Deliverables

| Deliverable | Access Link / Path | Description |
| :--- | :--- | :--- |
| **Live Web Application** | [earth-in-motion-nasa.base44.app](https://earth-in-motion-nasa.base44.app/) | Interactive NISAR telemetry and hazard exploration platform |
| **30-Second Demo Video** | [https://youtu.be/mSTLJCOyCpY | Overview of orbital mechanics, radar physics, and case studies *(replace with YouTube/Drive URL)* |
| **7-Slide Pitch Deck** | [View Presentation (PDF)](./docs/pitch-deck.pdf) | Executive summary, technical architecture, and scientific impact |

---

## About the Project

**Earth in Motion** is an interactive Earth-observation web platform built around the **NASA-ISRO Synthetic Aperture Radar (NISAR)** mission. Traditional optical satellites are obstructed by cloud cover, wildfire smoke, and darkness—leaving up to 70% of Earth's surface obscured at any given moment. Earth in Motion bridges raw orbital radar science and public accessibility by demonstrating how dual-frequency SAR penetrates atmospheric and vegetative barriers to measure millimeter-scale surface deformation.

### Platform Modules & Architecture

1. **01. The Mission**  
   Details NISAR's dual-frequency radar payload: a **24 cm L-Band antenna (1.257 GHz)** capable of penetrating dense forest canopies and dry soil, paired with a **12 cm S-Band antenna (3.20 GHz)** that resolves surface structures, crops, and snowpack across a **240 km SweepSAR swath** on a **12-day global repeat cycle**.
2. **02. Earth Explorer**  
   Interactive orbital telemetry visualization illustrating satellite pass geometry, swath coverage, and Interferometric SAR (InSAR) surface displacement measurements at sub-centimeter (`< 1 cm`) precision.
3. **03. Scientific Chapters**  
   Structured educational modules explaining SAR signal behavior, polarization (HH/HV), backscatter intensity, and interferometric phase coherence.
4. **04. Radar Workbench**  
   Interactive parameter exploration demonstrating how wavelength, incidence angle, and surface roughness govern radar returns across water, vegetation, ice, and urban infrastructure.
5. **05. Zoom to Issue (Global Case Studies)**  
   Target-lock hazard analyses utilizing NISAR Level-2 data products:
   * **Flood Intelligence — Brahmaputra (`26.20° N, 91.50° E`):** Maps monsoon water inundation beneath cloud cover via specular HH reflection (`NISAR_L2_GCOV`, Ascending Track 84).
   * **Wildfire & Forest Change — Rim Fire (`37.85° N, 120.05° W`):** Quantifies thermal canopy loss using HV depolarization (`NISAR_L2_GOFF`, Descending Track 27).
   * **Oil Slicks — Gulf of Mexico (`27.40° N, 90.60° W`):** Detects ocean surface roughness damping and slick transport (`NISAR_L2_GCOV`, Ascending Track 61, Coherence `0.31`).
   * **Glacial Motion — Pine Island Glacier (`75.00° S, 100.00° W`):** Tracks ice-sheet velocity fields via speckle and offset tracking (`NISAR_L2_GOFF`, Descending Track 119, Coherence `0.71`).
   * **Land Subsidence — Central Valley (`36.50° N, 119.60° W`):** Monitors aquifer compaction and vertical deformation via differential InSAR phase unwrapping (`NISAR_L2_GUNW`, Ascending Track 33, Coherence `0.83`).

---

## Repository Structure

```text
earth-in-motion-nasa/
├── README.md               # Project overview, mission specs, deliverables, and team roster
├── LICENSE                 # MIT open-source license
├── docs/
│   └── pitch-deck.pdf      # 7-slide NASA Space Apps presentation
└── demo/
    └── demo-video.mp4      # 30-second project demonstration video
```

---

## About the Team

We are a student STEM team focused on Earth observation, remote sensing, and developing accessible scientific visualization tools using open NASA data.

| Name | Role |
| :--- | :--- |
| **Hamdan Sayed** | Team Owner & Project Lead |
| **Marmik Raje** | Team Member |
| **Ahil Ashraf Pulikkalakath** | Team Member |
| **Mohamed Anas Ismail** | Team Member |
| **Tony Mario** | Team Member |
| **Nahyan Moothedath** | Team Member |

---

## Data & Mission References

* **NASA-ISRO SAR (NISAR) Mission Specifications:** Jet Propulsion Laboratory (JPL) / ISRO Dual-Frequency L-Band & S-Band Radar Parameters (`NISAR_L2_GCOV`, `NISAR_L2_GOFF`, `NISAR_L2_GUNW`).
* **Application Platform:** Hosted at [https://earth-in-motion-nasa.base44.app/](https://earth-in-motion-nasa.base44.app/).
