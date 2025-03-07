# Transport Accessibility Analysis of Public Transport Victoria (PTV)

## Project Overview
This project analyzes the accessibility of public transport within the Melbourne Metropolitan area by examining the spatial distribution and density of public transport routes and stops (bus, tram, and train). The analysis aims to reveal transport connectivity gaps and highlight opportunities for enhancing equitable accessibility throughout Melbourne.

## Objectives
- Evaluate the spatial distribution of public transport routes across Melbourne.
- Assess transport accessibility by analyzing the density of transport stops.
- Identify well-connected regions and underserved areas.
- Propose recommendations for improving transport accessibility.

## Methodology

### Data Sources
- **GTFS Data**: Detailed information on public transport stops, routes, schedules, and trips.
- **Australian Boundary Datasets (ABS)**: Geographic context for spatial analysis.

### Tools and Software
- **PostgreSQL with PostGIS Extension**: Data management, spatial queries, and processing.
- **QGIS**: Visualization of spatial data (route mapping and stop density).
- **Docker Terminal**: Data extraction and loading operations.

### Data Processing Steps
1. **Data Restoration**
   - Extracted and loaded GTFS data and boundary shapefiles into PostgreSQL.
   - Verified data integrity through structured queries.

2. **Data Preprocessing**
   - Filtered mesh blocks specific to Greater Melbourne.
   - Created polygonal boundaries for Melbourne Metropolitan Area.
   - Enhanced stop data with spatial attributes derived from latitude and longitude.

3. **Spatial Analysis**
   - Calculated stop density (stops per square kilometer).
   - Generated spatial visualizations for tram, train, and bus routes.

## Results
- **High Connectivity Areas**: Central Melbourne, benefiting from extensive and overlapping transport modes.
- **Underserved Regions**: Outer suburbs with sparse stop densities and limited route coverage, primarily reliant on bus services.

## Recommendations
- Enhance public transport infrastructure in outer suburbs to bridge connectivity gaps.
- Develop multi-modal transport hubs at strategic points to facilitate efficient commuter transitions between transport modes.
- Regular assessment and improvement of stop densities in lower-accessibility areas.

## How to Run
- Ensure Docker, PostgreSQL (PostGIS enabled), and QGIS are installed.
- Follow scripts provided in `scripts/` for data loading and preprocessing.
- Open QGIS project files (`.qgz`) for visualizations.

## Author
- Jay Panchal

## License

This project is licensed under the GNU General Public License v3.0. See the [LICENSE](LICENSE) file for details.

For further details, please consult the full report provided in `PTV Case Study Report.docx`.

