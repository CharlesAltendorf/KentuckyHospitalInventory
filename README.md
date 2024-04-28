# KentuckyHospitalInventory

## Intro
Jupyter notebook was used in conjunction with mapleaf python extention to create html file.  File contains heat map showing kentucky city points with 2016 population estimates and 115 registered "hospitals" as of 2021 with their "acute hospital beds" represented by the other heat map layer.

## Geojsons (both are from the KyGovMaps Open Data Portal)
1. Ky_Hosptials. https://opengisdata.ky.gov/datasets/kygeonet::ky-hospitals/about
   This layer has 115 active hospitals in Kentucky as of 2021.  I used the Acute Beds field in the html.  In the notebook for more analysis I use the operator and psych bed fields.
2. Kentucky_City_Points. https://opengisdata.ky.gov/datasets/kygeonet::kentucky-city-points/about
   This layer has 416 city points in Kentucky.  Up date as of 2022.  Two cities were excluded from html because they were throwing errors by technically having no registered population.  2016 population estimated field was most recent so it was used in htal.

## CSVs (Some csvs were created to help mapleaf python code run easier)

1. KentuckyHospitals. Acute, Pysch Bed totals were added with WGS 1984 x, y coordinates.
2. KentuckyCities. 2016 population estimates were added with WGS 1984 x, y coordinates.
