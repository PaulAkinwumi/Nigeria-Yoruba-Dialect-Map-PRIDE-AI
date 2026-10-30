# Nigeria Yoruba Dialect Map (PRIDE AI)

**V1 - Yoruba dialect variations across southwest Nigeria**

An interactive, single-page reference map of Yoruba dialect records across southwest Nigeria. The map shows major and local dialect records, all Nigerian states, and the national outline, with search, layer controls, and a detail panel for each record.

## Features

- 31 dialect records: 15 major and 16 local.
- All 36 states plus the Federal Capital Territory shown for context.
- Search by dialect, state, locality, family, or recorded varieties.
- Toggle major records, local records, and state boundaries.
- "Data area" and "Nigeria" view controls.
- Responsive layout for desktop, tablet, and mobile.
- Esri Light Gray Canvas basemap with no API key.
- No build step: the app is a single self-contained HTML file.

## Data and citation

The dialect records and state assignments are based on the supplied project workbook and the following source:

> Usman, A., & Falola, T. (2019). Geography and Society. In *The Yoruba from Prehistory to the Present* (pp. 1–28). Cambridge: Cambridge University Press. https://www.cambridge.org/core/books/yoruba-from-prehistory-to-the-present/geography-and-society/CC682B3D24A7A9648C018BABC1E2EDEA

State boundaries are from geoBoundaries (GRID3, CC BY 4.0), simplified for display. Basemap tiles are provided by Esri.

Markers are illustrative locations within each recorded state. They are not surveyed dialect boundaries.

## Notes

- The page uses CDN-hosted Leaflet, MarkerCluster, Tailwind CSS, and Google Fonts, so it needs an internet connection.
- No API keys or environment variables are required.
- A `LICENSE` file is optional. Add one only if you want to grant others explicit permission to reuse the code.
