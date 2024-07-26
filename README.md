# Unveiling the Dynamics of European Train Travel

This code is a Python script that performs data manipulation and visualization on a dataset of rail passengers. It uses various libraries such as pandas, seaborn, matplotlib, pycountry, pypopulation, and CountryInfo to handle the data and create visualizations.

## List of Required Files
- rail_passengers_total.csv
- rail_passengers_kilometers_total.csv
- road_eqs_carhab.csv

These files are included in the zip folder.

Source: [Eurostat](https://ec.europa.eu/eurostat)

## Data Manipulation
The script starts by importing the necessary libraries and reading the data from "rail_passengers_total.csv". It then manipulates the data by transforming it into a long format using the `melt()` function from pandas. The passenger values are converted to numeric format and stored in the "Passengers" column. ISO codes are added to the dataset using the pycountry library based on country names. Population values are obtained using the pypopulation library and added to the dataset. Area information is retrieved using the CountryInfo class from the CountryInfo library based on ISO codes. Missing ISO codes for Turkey are manually added. The script also handles missing population values by setting them to None. Area values for Montenegro, Czechia, and North Macedonia are manually added as they were missing. The script also adds the EU membership status for each country based on the accession year information provided.
