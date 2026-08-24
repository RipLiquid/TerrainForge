# Data

This directory contains the geospatial data required by the QGIS project.

## Files

### `terrain_vectors.gpkg`

A GeoPackage containing the CanVec vector layers used in the final maps:

- `contours`
- `elevation_points`
- `residential_areas`
- `roads`
- `waterbodies`
- `watercourses`
- `wooded_areas`

The original shapefiles were consolidated into a GeoPackage for a cleaner, more portable repository structure. Feature geometries and source attributes used by the QGIS project were retained.

### `dem.tif`

Canadian Digital Elevation Model raster used for the hypsometric terrain visualization.

### `hillshade.tif`

Hillshade raster used to enhance the visual representation of terrain relief.

## Source

**Government of Canada — Natural Resources Canada**

Datasets used:

- CanVec digital topographic data
- Canadian Digital Elevation Model (CDEM)

The metadata distributed with the source datasets identifies the **Open Government Licence – Canada** as the applicable licence. The Government of Canada datasets remain subject to their original licence and attribution requirements.

Source portal: https://maps.canada.ca/

Licence: https://open.canada.ca/en/open-government-licence-canada
