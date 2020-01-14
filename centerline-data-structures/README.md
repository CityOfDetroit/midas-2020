# Centerline data structures

## Project statement

We're developing a centerline file for use by the city, as we don't have a common centerline file; most users at the city are using some variant of the Michigan Geographic Framework, available [here](https://gis-michigan.opendata.arcgis.com/datasets/all-roads-v17a). Currently, we are strictly a consumer of the MGF but eventually we should be feeding updates from our internal centerline back to the MGF.

Here's a few of the areas where we use this data:
- 911/emergency services routing/geocoding
- pavement condition
- road closures for events or construction
- right-of-way permits

While we're gathering requirements internally from each department, we should look at how other cities manage this data. The scope of this data is broad and can encompass the entire right-of-way. Cities might publish:

- Centerline files (a polyline file describing the center of the road)
- Curbline files (a polygon file representing the paved surface of the road from curb-to-curb)
- Other types of files that we don't know about

## Resources/Examples

- Philadelphia publishes a curbline file: https://www.opendataphilly.org/dataset/curb-edges
- The US Census publishes the TIGER/LINE shapefiles: https://www.census.gov/cgi-bin/geo/shapefiles/index.php
- OpenStreetMap publishes a global centerline dataset - you can [download an extract for the metro area here](https://www.interline.io/osm/extracts/)
- SEMCOG has published sidewalks and crosswalks (ask for download)

## Desired outcome

- We'd like a better understanding of how other cities are managing this data: 
  - what attributes should be included?
  - what type of feature should they be attached to?
- Can we develop a 'crosswalk' among different datasets?
