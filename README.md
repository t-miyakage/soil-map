# Vietnam Soil Map / ベトナム土壌図マップ / Bản đồ Đất Việt Nam

A free, browser-based soil map viewer for Vietnam. Upload a KML file to see the soil classification of any area.

KMLファイルをアップロードして、ベトナムの任意のエリアの土壌分類を確認できる無料のWebアプリです。

Ứng dụng web miễn phí để xem bản đồ đất Việt Nam. Tải lên tệp KML để xem phân loại đất của bất kỳ khu vực nào.

## Features / 機能

- **KML File Upload** — Drag & drop or select a KML file to display the area boundary on the map
- **WRB Soil Classification** — World Reference Base soil type overlay (ISRIC SoilGrids 250m)
- **Soil pH** — Surface (0-5cm) soil pH layer
- **Trilingual UI** — Japanese / English / Vietnamese
- **Multiple Base Maps** — OpenStreetMap, Esri Satellite, OpenTopoMap, CartoDB Dark
- **Click to Identify** — Click anywhere on the map to get soil info for that point

## Data Sources / データソース

| Layer | Source | Resolution |
|-------|--------|------------|
| WRB Soil Classification | [ISRIC SoilGrids 250m v2.0](https://soilgrids.org/) | 250m |
| Soil pH (0-5cm) | [ISRIC SoilGrids 250m v2.0](https://soilgrids.org/) | 250m |
| Base Maps | OpenStreetMap, Esri, OpenTopoMap, CARTO | — |

## Usage / 使い方

1. Open the app in a browser
2. Upload a KML file (drag & drop or click the upload area)
3. Select a soil layer (WRB or pH)
4. Click on the map to view detailed soil info
5. Switch language using the buttons at the top of the panel

## Tech Stack

- [Leaflet](https://leafletjs.com/) — Map rendering
- [toGeoJSON](https://github.com/tmcw/togeojson) — KML parsing
- ISRIC SoilGrids WMS — Soil data layers
- Pure HTML/CSS/JS — No build step required

## Deployment

This is a single `index.html` file. Deploy to any static hosting:

```bash
# GitHub Pages
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/vietnam-soil-map.git
git push -u origin main
# Then enable GitHub Pages in Settings → Pages → Source: main branch
```

## License

MIT License — Free to use, modify, and distribute.
