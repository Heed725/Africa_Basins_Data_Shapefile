# Africa Basins Data Shapefile

A collection of geospatial shapefiles containing hydrological data for the African continent, including river basin boundaries and river networks.

## 📁 Contents

| File | Description |
|------|-------------|
| `hydrobasins_africa.zip` | HydroBASINS data for Africa - watershed boundaries at multiple hierarchical levels |
| `rivers_africa_37333.zip` | African river network shapefile data |

## 🌍 About the Data

### HydroBASINS Africa
HydroBASINS provides a series of polygon layers depicting watershed boundaries at multiple scales. The data is derived from the HydroSHEDS database and provides a consistent, hierarchical system of nested sub-basins for the African continent.

### Rivers Africa
This dataset contains the river network geometry for Africa, useful for hydrological analysis, water resource management, and environmental studies.

## 🚀 Usage

1. Download the ZIP files from this repository
2. Extract the contents to access the shapefile components (`.shp`, `.shx`, `.dbf`, `.prj`, etc.)
3. Load into your preferred GIS software:
   - QGIS (free, open-source)
   - ArcGIS
   - Python (using `geopandas`, `shapely`, `fiona`)
   - R (using `sf` package)

### Example with Python

```python
import geopandas as gpd

# Load the hydrobasins shapefile
basins = gpd.read_file("hydrobasins_africa.shp")

# Load the rivers shapefile
rivers = gpd.read_file("rivers_africa_37333.shp")

# Display basic info
print(basins.info())
print(rivers.info())

# Plot the data
basins.plot()
rivers.plot()
```

## 📊 Applications

- Hydrological modeling and analysis
- Water resource management
- Flood risk assessment
- Environmental impact studies
- Climate change research
- Agricultural planning
- Infrastructure development

## 📜 License

Please refer to the original data sources for licensing information:
- [HydroSHEDS / HydroBASINS](https://www.hydrosheds.org/) - WWF

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report issues
- Submit pull requests
- Suggest improvements

## 📬 Contact

For questions or suggestions, please open an issue in this repository.

---

**Note:** These datasets are intended for research and educational purposes. Always verify data accuracy for critical applications.
