# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-06-24

### Added
- **Module 01:** Implemented the Multi-Commodity Capacitated Facility Location Problem (MC-CFLP) for network rightsizing, featuring minimum workload constraints to prevent inefficient facility openings.
- **Module 02:** Integrated the Capacitated Location-Routing Problem (CLRP) to optimize both facility locations and vehicle dispatch routes simultaneously.
- **Module 03:** Developed a Multi-Period Dynamic Facility Location Problem (MP-DFLP) model to generate 3-to-5-year strategic CapEx investment roadmaps.
- **Module 04:** Introduced a Two-Stage Stochastic Facility Location Problem (SFLP) to handle demand uncertainty and mitigate supply chain disruptions (Stock-outs).
- Formulated Miller-Tucker-Zemlin (MTZ) constraints to eliminate sub-tours in vehicle routing.
- Integrated `folium.plugins.AntPath` for animated, directional route mapping.
- Added automated diagnostic reporting systems (Actionable Insights) based on utilization thresholds.

### Changed
- Refactored single-product binary assignment variables to multi-product continuous flow variables for realistic capacity management.
- Upgraded static visual plots to dynamic, multi-scenario NetworkX dashboards (Wait-and-See phase analysis).
- Shifted coordinate centers to Ho Chi Minh City for localized case studies.