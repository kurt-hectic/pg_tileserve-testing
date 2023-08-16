# pg_tileserve-testing
Jupyter notebook with code to test if vector tiles returned by pg_tileserv in WDQMS are the same as in old implementation

## approach
The script fetches all tiles of a layer at a given zoom level from the old and new systems. Using a vector tile library it extracts all features from these tiles and then checks if the same features are present in both systems using pandas dataframes. Vector tile internal coordinates are used as index and relevant payload fields are used for the comparison.  

## installation
The ```mapbox_vector_tile, requests and pandas``` libraries are needed.
