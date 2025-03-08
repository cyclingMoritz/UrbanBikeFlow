# Data Structure

This document provides an overview of the data structure and the contents of each folder in the `reallocate_bcn_pilot1` project.

## Folder Structure

The data is organized into the following folders:

- `external/`
    - Contains data from external sources.
- `raw/`
    - Contains the raw data files as received from the data sources.
- `interim/`
    - Contains intermediate data that has been transformed but not yet fully processed.
- `processed/`
    - Contains the processed data files after initial cleaning and transformation.

## Documentation

### external/

#### accidents/
- `2023-2010_accidents_persones_FINAL.xlsx`
    - Description: Contains the received about people hurt in accidents from 2023 to 2010 in excel.
    - Columns:  `FileNumber`, `District code`, `District name`, `Code area`, `Name area`, `Street code`, `Street name`, `Postal number`, `Weekday`, `Year`, `Month number`, `Month name`, `Day`, `Daytime`, `Hour`, `Cause of accident for pedestrian`, `Descrip. of accident opponent`, `Gender/Sex`, `Age`, `Person type`, `Accident location pedestrian`, `Descrip. motiv/activity pedestrian`, `Descrip. motiv/activity Driver`, `Injury severity`, `Coordenada_UTM_X_ED50`, `Coordenada_UTM_Y_ED50`, `Latitud_WGS84`, `Longitud_WGS84`, `Latitud_WGS84.1`, `Longitud_WGS84.1`, `Coordinates number`
- `2023-2010_accidents_vehicles_FINAL.xlsx`
    - Description: Contains the received about vehicles involved in accidents from 2023 to 2010 in excel.
    - Columns: `FileNumber`, `District code`, `District name`, `Code area`, `Name area`, `Street code`, `Street name`, `Postal number`, `Weekday`, `Year`, `Month number`, `Month name`, `Day`, `Hour`, `Daytime`, `Cause of accident for pedestrian`, `Vehicle type`, `Vehicle model`, `Manufacture`, `Color`, `License type`, `Possession of driving license in years`, `Coordenada_UTM_X_ED50`, `Coordenada_UTM_Y_ED50`, `Latitud_WGS84`, `Longitud_WGS84`, `Latitud_WGS84.1`, `Longitud_WGS84.1`, `Coordinates number`

#### emplacaments

- `REALLOCATE_emplacaments.shp`
    - Description: Shapefile with the polygons of the superilles we want to study.
    - Columns: `fid`, `ESTAT_maig`, `NOM`, `FINALITZAC` 

<!-- ### raw/

- `2023-2010_accidents_persones_FINAL.xlsx`
    - Description: Contains the received data w
    - Columns: `column1`, `column2`, `column3`
- `2023-2010_accidents_vehicles_FINAL.xlsx`
    - Description: Contains raw data from source 2.
    - Columns: `columnA`, `columnB`, `columnC` -->

### interim/

- `accidents_persones-2023_2010.parquet`
    - Description: Intermediate data from *2023-2010_accidents_persones_FINAL.xlsx*
    - Columns: `FileNumber`, `District code`, `District name`, `Code area`, `Name area`, `Street code`, `Street name`, `Postal number`, `Weekday`, `Year`, `Month number`, `Month name`, `Day`, `Daytime`, `Hour`, `Cause of accident for pedestrian`, `Descrip. of accident opponent`, `Gender/Sex`, `Age`, `Person type`, `Accident location pedestrian`, `Descrip. motiv/activity pedestrian`, `Descrip. motiv/activity Driver`, `Injury severity`, `Coordenada_UTM_X_ED50`, `Coordenada_UTM_Y_ED50`, `Latitud_WGS84`, `Longitud_WGS84`, `Latitud_WGS84.1`, `Longitud_WGS84.1`, `Coordinates number`
- `interim_data2.csv`
    - Description: Intermediate data from *2023-2010_accidents_vehicles_FINAL.xlsx*
    - Columns: `FileNumber`, `District code`, `District name`, `Code area`, `Name area`, `Street code`, `Street name`, `Postal number`, `Weekday`, `Year`, `Month number`, `Month name`, `Day`, `Hour`, `Daytime`, `Cause of accident for pedestrian`, `Vehicle type`, `Vehicle model`, `Manufacture`, `Color`, `License type`, `Possession of driving license in years`, `Coordenada_UTM_X_ED50`, `Coordenada_UTM_Y_ED50`, `Latitud_WGS84`, `Longitud_WGS84`, `Latitud_WGS84.1`, `Longitud_WGS84.1`, `Coordinates number`

### processed/

- `cleaned_data1.csv`
    - Description: Cleaned data from source 1.
    - Columns: `column1`, `column2`, `column3`
- `cleaned_data2.csv`
    - Description: Cleaned data from source 2.
    - Columns: `columnA`, `columnB`, `columnC`

