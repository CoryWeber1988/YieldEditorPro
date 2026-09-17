# Changelog

All notable changes to this project are documented here. Dates are in `YYYY-MM-DD`.

## [Unreleased]

### Added
- Open-source release: README, AGPLv3 license, contributing guide, and this changelog.
- Drag-to-reorder filter list, with a checkbox to switch between the traditional fixed USDA filter order and a user-defined order.
- Streamlined export column-set option — export just the cleaned wet/dry/moisture values under their *original* column names, alongside the existing "Full" (original + cleaned columns) export.
- Ordinary Kriging as an alternative to IDW for GeoTIFF raster interpolation, with an optional manual variogram range.
- Esri Aerial Imagery Hybrid basemap (imagery + labels overlay), plus OpenTopoMap and Humanitarian OSM basemap options.
- In-app Help tab sections: tool overview, USDA Yield Editor attribution, and developer/contact info.

### Changed
- Removed CARTO basemap options (they require an API key, which doesn't fit a single keyless HTML file).
- Moved the map zoom (+/−) control from the top-left to the bottom-left, so it no longer overlaps the "Colour map by" panel.

### Earlier
- Separate, independently-optional Dry/Processed Yield and Wet/Unprocessed Yield column mapping, with a user-chosen primary yield column driving filters and pass-outlier detection.
- Core pipeline: Import (AgLeader Text / CSV / GeoJSON / Shapefile), column-mapping auto-detection, date/machine/moisture Balance, the full USDA Yield Editor Filter set, Post-Cal scale-total calibration, boundary import, and CSV/GeoJSON/Shapefile/AgLeader Text/GeoTIFF export.
- Session save/load, and a downloadable Markdown/HTML summary report.
