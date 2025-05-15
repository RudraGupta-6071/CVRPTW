# Optimizing Waste Collection and Disposal Routing  
**A Multi‑Phase Vehicle Routing Approach Using Google OR‑Tools**

## 📖 Project Overview  
Municipal waste management is a critical urban service that often suffers from high operational costs, suboptimal vehicle utilization, and increased environmental impact. This project develops and implements a **two‑phase Vehicle Routing Problem (VRP) model** for waste collection and disposal, integrating collection from distributed bins and transport to final disposal sites into a single, cohesive optimization framework. We leverage Google OR‑Tools to generate near‑optimal routes under realistic capacity, time‑window, and transfer‑station constraints :contentReference[oaicite:0]{index=0}:contentReference[oaicite:1]{index=1}.

## 🎯 Objectives  
1. **Minimize Total Operation Time** – including driving, waiting, and service durations.  
2. **Maximize Vehicle Utilization** – ensuring no vehicle exceeds capacity while minimizing unused fleet size.  
3. **Honor Time Windows** – comply with collection/disposal slot restrictions in urban areas.  
4. **Balance Workload** – evenly distribute service tasks across the fleet. :contentReference[oaicite:2]{index=2}:contentReference[oaicite:3]{index=3}

## 📐 Methodology  
- **Phase 1: Collection Routing**  
  - 17×17 time matrix, 4 vehicles (capacity 20 units), pick‑up from bins → transfer stations.  
- **Phase 2: Disposal Routing**  
  - 21×21 time matrix, 5 vehicles (capacity 7 units), transport from transfer stations → disposal sites.  
- **Solver:** Google OR‑Tools 9.6 via Python 3.11  
- **Development Stack:** NumPy, Pandas, GeoPandas, Matplotlib, Folium :contentReference[oaicite:4]{index=4}:contentReference[oaicite:5]{index=5}

## 💾 Dataset  
This repository includes a synthetic dataset reflecting real‑world constraints:  
- **Travel Times:** Two static matrices (17×17 for pick‑up, 21×21 for delivery).  
- **Demands & Time Windows:** Node‑level demands and service windows.  
- **Scalability:** Easily extendable to larger instances or real GIS data. :contentReference[oaicite:6]{index=6}:contentReference[oaicite:7]{index=7}
