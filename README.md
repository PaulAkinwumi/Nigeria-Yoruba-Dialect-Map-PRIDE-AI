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

## Run locally

From this folder:

```bash
python3 -m http.server 8000
```

Then open <http://localhost:8000>.

You can also open `index.html` directly in a browser, but a local server is recommended so relative files and browser security rules behave consistently.

## Deploy to GitHub Pages

1. Create a new empty repository on GitHub. Do not add a README or `.gitignore` there because they are already in this folder.
2. In this folder, initialize Git and push:

```bash
git init
git add .
git commit -m "Build Nigeria Yoruba dialect map"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
git push -u origin main
```

3. On GitHub, open **Settings → Pages**.
4. Under **Build and deployment**, set **Source** to **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then click **Save**.
6. Wait for the deployment to finish. The site will be available at:

```text
https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/
```

`index.html` must stay at the repository root for GitHub Pages to serve it automatically.

## Project structure

```text
.
├── index.html
├── README.md
├── .gitignore
└── Yoruba dialects and their states.xlsx
```

The workbook is the source data and is not required by the live page, because the map data is embedded in `index.html`.

## Notes

- The page uses CDN-hosted Leaflet, MarkerCluster, Tailwind CSS, and Google Fonts, so it needs an internet connection.
- No API keys or environment variables are required.
- A `LICENSE` file is optional. Add one only if you want to grant others explicit permission to reuse the code.
