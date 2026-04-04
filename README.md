# 🌱 Agroecological Crop Suitability & Food Vulnerability Mapping
**Central America · Python/GIS + Power BI · 2026**

**Author:** Saúl Chaves Barrantes — Food Engineer & Data Scientist  
**Stack:** Python · GeoPandas · Folium · Power BI  
**Data sources:** WorldClim 2.1 · SoilGrids · FAOSTAT · IPCC AR6  

---

## Objective

End-to-end geospatial analysis assessing agroecological crop suitability
and food vulnerability across 7 Central American countries, with
climate-change projections under SSP2-4.5 (2041–2060).

---

## Key Outputs

| Output | Description |
|--------|-------------|
| **Agroecological Suitability Index (ASI)** | Weighted overlay: temperature · precipitation · soil pH |
| **Food Vulnerability Index (FVI)** | Undernourishment · import dependency · rural poverty |
| **Climate Risk Assessment** | ASI delta under SSP2-4.5 vs 1970–2000 baseline |
| **Interactive Map** | Folium choropleth — FVI + ASI layers · country popups |
| **Power BI Dashboard** | 6 visuals · slicers · KPI cards |

---

## Methodology

**Crop suitability** — FAO GAEZ v4 framework, 5 crops:
Maize · Coffee Arabica · Rice · Common Bean · Sugarcane

**ASI:**  `(temp_score × 0.40) + (precip_score × 0.40) + (soil_score × 0.20)`

**FVI:**  `(undernourishment × 0.50) + (import_dependency × 0.25) + (rural_poverty × 0.25)`

**Climate scenario:** IPCC AR6 SSP2-4.5 — Central America regional deltas

---

## Key Findings

- 🔴 Nicaragua, Honduras and Guatemala — highest food vulnerability (FVI > 0.60)
- 🌡️ Coffee Arabica in El Salvador — highest climate risk under SSP2-4.5
- 🌱 Costa Rica and Panama — strongest agroecological suitability
- ⚠️ All 7 countries show negative ASI delta under mid-century warming scenario

---

## Data Sources

- WorldClim 2.1 — historical climate averages
- SoilGrids — soil pH, clay, organic carbon
- FAO GAEZ v4 — crop suitability parameters  
- FAOSTAT — undernourishment, food balance
- World Bank — rural poverty indicators
- IPCC AR6 WGI — SSP2-4.5 regional projections
- Natural Earth — administrative boundaries
