# Methodology

## Study Area

The map extent covers part of the Hamilton–Burlington region of southern Ontario, including portions of the Niagara Escarpment and the western Lake Ontario shoreline.

## Coordinate Reference System

The final layouts use **NAD83 / UTM Zone 17N**, an appropriate projected coordinate system for local-scale mapping in this part of Ontario. Both maps were designed at a scale of **1:50,000**.

## Topographic Map

The topographic map combines seven CanVec vector themes:

- contours;
- elevation points;
- residential areas;
- road segments;
- waterbodies;
- watercourses; and
- wooded areas.

Index contours were distinguished from interval contours using the contour elevation field, and selected index contours were labeled to improve terrain interpretation. Transportation, hydrography, vegetation, and residential land cover were symbolized to provide reference information without overwhelming the elevation features.

## Terrain Map

The terrain map combines raster elevation data with vector reference layers.

The DEM was rendered with a hypsometric colour ramp so lower elevations appear greener and progressively higher terrain shifts through earth tones toward lighter colours. Hillshade was placed above the DEM with partial transparency and a multiply blend, strengthening local relief while preserving the underlying elevation colours.

Roads, watercourses, waterbodies, residential areas, wooded areas, and selected contour labels were layered above the raster terrain. Their styling was intentionally subdued so the elevation surface remained visually dominant.

## Cartographic Design

Both layouts include a title, north arrow, scale information, legend, projection information, and data-source attribution. The topographic map prioritizes precise contour interpretation, while the terrain map prioritizes rapid visual understanding of landform and the relationship between relief, vegetation, and developed areas.

## Repository Packaging

The original course dataset contained many CanVec feature classes that were not used in the final maps. For this portfolio repository, only the seven vector layers referenced by the QGIS project were retained and consolidated into `terrain_vectors.gpkg`. The DEM and hillshade remain as GeoTIFF rasters.

This reduces repository size and makes the project easier to clone, inspect, and reproduce without changing the analytical or cartographic content used in the maps.
