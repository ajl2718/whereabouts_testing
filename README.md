# Comparison of accuracy and latency of whereabouts with other geocoders
This repo contains data and code for testing the accuracy and speed of whereabouts compared with three other geocoding solutions.

## Comparison geocoders
Three geocoders for comparison are: [Google Geocoding API](https://developers.google.com/maps/documentation/geocoding/overview), [Mapbox Geocoding API](https://docs.mapbox.com/api/search/geocoding/) and [Nominatim](https://nominatim.org/).


## Datasets
Three datasets are used for comparison
- Residential properties in Australia: rea_130824.csv
- Business locations in Australia: gyg_210624_geocoded.csv
- Licensed venues in the state of Victoria, Australia: liquor.xlsx. This is from [VicGov's Open Data Portal](https://discover.data.vic.gov.au/dataset/victorian-liquor-licences-by-location)

The first two datasets are used to assess accuracy while the third is to measure speed.

## Code
The notebook `geocoder_comparison_220425.ipynb` contains the code to compare the performance of geocoding algorithms on these two datasets.

## Methodology
For each geocoded address, the results are compared with the true address at the apartment, street number, street name and suburb level. Each address is manually reviewed to create the results for the accuracy at each level of granularity.

## License disclaimer
The datasets are used solely for testing geocoding performance and should only be used subject to license restrictions. 