# gadm-census-correspondence
This is a corresppondence table to match Canadian census division data from Statistics Canada and [GADM](https://gadm.org/download_country_v3.html).

Statistics Canada uses a `CDUID` unique identifier for census divisions, while GADM uses its own standard.

For example, the census division for Antigonish in Nova Scotia has the `CDUID` of 1214, while GADM identifies it as CAN.7.2_1 in the `GID_2` column.

This is handy if you want to join Canadian census data to other datasets using the GADM identifier (for example, [Facebook mobility data](https://dataforgood.fb.com/docs/covid19/#covid-19-mobility-data-network)).

This correspondence table is not perfect. Some GADM geographies are outdated, especially in Quebec, British Columbia and the Northwest Territories. Some census divisions have since been split into multiple, like Centre-de-la-Mauricie in Quebec and Comox-Strathcona in B.C. Use with caution.

This table was created by running a spatial join on census division shapefiles from Statistics Canada and GADM. Mismatched features from overlapping borders were corrected manually.
