# 🌐 Enterprise Supply Chain Network Optimization Suite

[![Python 3.10+](https://img.shields.io/badge/python-3.10+-blue.svg)](https://www.python.org/downloads/)
[![PuLP](https://img.shields.io/badge/Optimization-PuLP-orange.svg)](https://coin-or.github.io/pulp/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Maintained](https://img.shields.io/badge/Maintained%3F-yes-brightgreen.svg)](https://github.com/yourusername/Supply-Chain-Network-Optimization)

> An advanced Operations Research (OR) toolkit designed to solve complex logistics, warehousing, and routing challenges using Mixed-Integer Linear Programming (MILP).

## 📊 Executive Summary

This repository contains a collection of mathematical optimization models that mirror the core network design systems used by leading global e-commerce and logistics corporations. Moving beyond basic deterministic algorithms, this suite addresses real-world constraints such as multi-commodity capacity, vehicle routing subtour elimination, long-term dynamic investments, and stochastic demand uncertainty.

---

## 🏗️ Project Architecture & Mathematical Models

This project is divided into four distinct sub-modules, progressively scaling in complexity and strategic depth. **All models are formulated based on industry-standard Operations Research frameworks.**

### 1. `01_MC_CFLP_Rightsizing`
**Model:** Multi-Commodity Capacitated Facility Location Problem (MC-CFLP)
* **Use Case:** Strategic network rightsizing and capacity planning.
* **Features:** Handles multiple product types (e.g., Dry vs. Cold storage) with continuous flow variables. Incorporates *Minimum Workload Constraints* to identify underutilized facilities for consolidation and avoid opening financially unviable sites.
* **Output:** Stacked bar diagnostic dashboards with automated actionable insights.

### 2. `02_CLRP_Routing`
**Model:** Capacitated Location-Routing Problem (CLRP)
* **Use Case:** Simultaneous optimization of facility locations and last-mile vehicle dispatch routes.
* **Features:** Integrates the classical Facility Location Problem with the Vehicle Routing Problem (VRP). Utilizes **Miller-Tucker-Zemlin (MTZ)** constraints to eliminate sub-tours and enforce vehicle capacity limits.
* **Output:** Interactive, animated GIS maps using Folium `AntPath` to visualize directional dispatch sequences.

### 3. `03_MP_DFLP_Roadmap`
**Model:** Multi-Period Dynamic Facility Location Problem (MP-DFLP)
* **Use Case:** Long-term CapEx investment planning (3-5 year roadmap).
* **Features:** Introduces the element of time. The algorithm balances operating costs against the penalty of breaking leases (closing costs) and opening new mega-facilities over multiple time periods.
* **Output:** Network evolution graph visualizing demand vs. capacity dynamics over time.

### 4. `04_SFLP_Stochastic`
**Model:** Two-Stage Stochastic Facility Location Problem (SFLP)
* **Use Case:** Supply chain risk management and resilience planning.
* **Features:** Replaces deterministic demand with probabilistic scenarios (Normal, Peak, Crisis). Balances the *Here-and-Now* fixed costs of opening warehouses against the *Wait-and-See* expected penalty costs of stock-outs during unexpected demand surges.
* **Output:** Parallel universe stress-test dashboards.

---

## 💻 Tech Stack

* **Optimization Engine:** `PuLP` (Linear & Integer Programming solver)
* **Geospatial Mapping:** `Folium`, `Leaflet` (Interactive HTML maps)
* **Data Manipulation:** `Pandas`, `NumPy`
* **Network Topology & Visualization:** `NetworkX`, `Matplotlib`

---

## 🚀 Installation & Usage

**1. Clone the repository:**
```bash
git clone [https://github.com/yourusername/Supply-Chain-Network-Optimization.git](https://github.com/yourusername/Supply-Chain-Network-Optimization.git)
cd Supply-Chain-Network-Optimization