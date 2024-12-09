### ⚠️ Special Note

> **IMPORTANT**  
> The code with the name "Final.ipynb" is for final submission
 

# **NYC Urban Analysis**

This repository contains a comprehensive spatial analysis of New York City (NYC), focusing on land use, accessibility, infrastructure, and urban dynamics. Using geospatial data and Python-based visualization tools, the project examines patterns in transportation, building heights, parking density, traffic hotspots, and Points of Interest (POIs).

---

## **Project Overview**

This project integrates multiple datasets and spatial analysis methods to understand NYC's urban structure. Key analyses include:
- **Land Use Distribution**: Examining the spatial organization of residential, commercial, and green spaces.
- **POI Accessibility**: Evaluating access to transportation networks, especially subway lines.
- **Traffic Hotspots**: Identifying high-congestion areas using Kernel Density Estimation (KDE).
- **Building Height Analysis**: Mapping vertical growth patterns across NYC.
- **Parking Density**: Visualizing parking availability across boroughs.
- **Service Void Detection**: Identifying areas with below-average POI density.
- **Voronoi Analysis**: Representing competitive zones for POIs.

---

## **Key Findings**

- **Land Use**: Residential zones dominate Staten Island and the Bronx, while Manhattan features a mix of residential, commercial, and recreational areas. Parks like Central Park provide critical urban greenery, and industrial zones are concentrated in Queens and Brooklyn.
- **Accessibility**: Manhattan leads in POI accessibility within 500 meters of subway lines, while Staten Island and the Bronx show significant gaps.
- **Traffic Hotspots**: Midtown Manhattan and Downtown Brooklyn are the most congested areas, with moderate congestion in Queens and the Bronx.
- **Building Heights**: Skyscrapers dominate Manhattan, while Brooklyn and Queens show moderate heights, and Staten Island is largely low-rise.
- **Parking**: Parking density is highest near commercial hubs and lower in residential zones.

---

## **Data Sources**

The analysis is based on the following datasets:

1. **Major Roads**: Line geometries of NYC’s primary streets.
2. **Subway Lines**: Comprehensive geometries of subway routes.
3. **Borough Boundaries**: Spatial extent of NYC’s boroughs.
4. **Points of Interest (POIs)**: Categorized into 13 facility types (e.g., residential, transportation, education).
5. **Building Boundaries**: Building footprints, heights, and construction years.
6. **Land Use**: Zoning and land use data for NYC.
7. **Parking Places**: Custom dataset mapping parking facilities.

---

## **Methods**

The project uses a range of spatial analysis techniques:
- **Proximity Analysis**: Evaluating accessibility to subway lines and major roads.
- **Kernel Density Estimation (KDE)**: Generating heatmaps for traffic and parking density.
- **Buffering**: Defining catchment areas for subway lines and other infrastructure.
- **Voronoi Diagrams**: Visualizing competition zones for POIs.
- **Service Void Detection**: Identifying underserved areas based on POI density.

Visualization tools include `geopandas`, `matplotlib`, `seaborn`, and `contextily` for basemap integration.

---

## **Features**

- **Land Use Distribution Map**: Visualizing NYC’s residential, commercial, and green spaces.
- **Traffic Hotspot Map**: KDE heatmap of congestion zones.
- **POI Accessibility Bar Charts**: Subway proximity analysis by borough.
- **Building Height Map**: Gradient map of vertical density.
- **Parking Accessibility Map**: Heatmap of parking availability.
- **Service Void Detection**: Highlighting areas with low POI density.

---

## **How to Run**

1. **Install Dependencies**:
   - Ensure Python 3.7+ is installed.
   - Install required libraries:
     ```bash
     pip install geopandas pandas matplotlib seaborn contextily shapely
     ```

2. **Clone the Repository**:
   ```bash
   git clone https://github.com/username/nyc-urban-analysis.git
   cd nyc-urban-analysis
   ```

3. **Prepare Data**:
   - Place the required shapefiles and CSV files in the `data/` folder.
   - Update file paths in the scripts.

4. **Run Analysis**:
   - Execute the analysis scripts:
     ```bash
     python analysis_script.py
     ```

5. **View Results**:
   - Figures and visualizations will be saved in the `output/` directory.

---

## **Repository Structure**

```
├── data/
│   ├── geo_export_*.shp         # Shapefiles for roads, subways, etc.
│   ├── parking_places.csv       # Parking facilities dataset
├── scripts/
│   ├── analysis_script.py       # Main analysis script
│   ├── visualization_helpers.py # Utility functions for plotting
├── output/
│   ├── land_use_distribution.png
│   ├── traffic_hotspots.png
│   ├── building_heights.png
│   ├── parking_density.png
├── README.md                    # Project documentation
```

---

## **Future Work**

- Expand accessibility analysis to include bus networks.
- Conduct temporal analysis of infrastructure growth.
- Improve POI categorization by incorporating additional facility types.

---

## **License**

This project is licensed under the [MIT License](LICENSE).

---

## **Acknowledgments**

Special thanks to NYC Open Data and the NYC Department of City Planning for providing the datasets used in this analysis.

---

Let me know if you'd like adjustments or additional sections!
