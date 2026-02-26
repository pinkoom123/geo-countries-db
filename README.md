# geo-countries-db
🌍 Comprehensive  world dataset of ~235 countries with ISO 3166-1 alpha-2/alpha-3 codes, UN M49 region/sub-region codes, dial codes, capitals, currencies, primary languages, land area (km²), nominal GDP (USD), and bounding box coordinates. Sourced from reliable geonames and UN standards for global mapping, data analysis, and geospatial applications. 
This is very useful for climate modelling and geospatial analysis, or mapping.
There is a Python script for easy access to information(bounding_boxes, regions,land areas,currencies and etc) for each country, if you don't prefer the raw text(JSON).


##  📁 Files

| File | Purpose | Format |
|------|---------|--------|
| `country_codes` | **Main dataset** - All country information | JSON |
| `Geo_countries.ipynb` | **Python module** - Easy programmatic access | Python |

##  🚀 Quick Start

**Direct access:**
```python
import json
with open('country_codes', 'r') as f:
    countries = json.load(f)
ghana = countries['gh']
print(ghana['capital'])  # Accra
