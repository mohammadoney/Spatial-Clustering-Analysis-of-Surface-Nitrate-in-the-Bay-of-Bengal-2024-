# Spatial-Clustering-Analysis-of-Surface-Nitrate-in-the-Bay-of-Bengal-2024-
This project analyzed the spatial distribution of surface nitrate concentrations in the Bay of Bengal for the year 2024, identifying statistically significant clusters of high and low values using advanced spatial statistics.

Step-by-Step Process:

Data Acquisition & Preprocessing:
Satellite-derived surface nitrate data (no3_depth1) from the Copernicus Marine Service was extracted for 2024.
A median composite was created to represent the central tendency of nitrate concentrations over the year, minimizing the influence of outliers or transient events.
The data was clipped to the Bay of Bengal region using a defined polygon.

Hotspot Analysis (Getis-Ord Gi*):
The Local Getis-Ord Gi* statistic was applied to the median nitrate raster. This tool identifies areas where high or low values cluster spatially more than would be expected by random chance.
It calculates a Z-score for each pixel: a high positive Z-score indicates a "hotspot" (cluster of high nitrate values), a high negative Z-score indicates a "coldspot" (cluster of low values), and scores near zero suggest no significant clustering.
A p-value is calculated to determine the statistical significance of each Z-score.

Pattern Identification & Real-World Interpretation:
The analysis revealed a dominant pattern of widespread, statistically significant coldspots (clusters of very low nitrate, ~0.01 mmol m⁻³) covering 42.6% of the analyzed area.
In contrast, hotspots were few, isolated, and extremely intense. The 99% confidence hotspots, though only 43 pixels, showed anomalously high nitrate concentrations (averaging ~39.6 mmol m⁻³).

Real-World Translation:
Coldspots: The vast areas of low nitrate align with the Bay of Bengal's well-known characteristic as an "oligotrophic" basin—a marine desert with chronically low nutrient levels, especially in surface waters offshore. This limits phytoplankton growth.
Intense, Localized Hotspots: The few intense hotspots likely correspond to major river plumes (e.g., from the Ganges-Brahmaputra, Irrawaddy, and Godavari rivers). These rivers discharge massive amounts of nutrients (including nitrate) into the coastal ocean, creating sharp, localized gradients and fertile patches that drive coastal productivity.
The stark contrast between the vast oceanic low-nutrient zones and the sharply defined, high-nutrient river plumes is a classic and ecologically critical feature of the Bay of Bengal's biogeochemistry.

Visualization & Communication:
A four-panel figure was created to effectively communicate both the raw data and the statistical results:
1) Raw median nitrate distribution.
2) Nitrate values only in statistically significant areas.
3) A classified hotspot/coldspot map.
4) A diverging map of Z-scores, highlighting significance.
