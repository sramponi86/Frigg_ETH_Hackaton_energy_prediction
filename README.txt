Data README

DE-LU_prices.csv / ES_prices.csv
  Source    : ENTSO-E Transparency Platform / energy-charts.info
  Variables : timestamp (UTC), price (EUR/MWh)
  Frequency : hourly
  Period    : 2022-01-01 to 2026-05-07
  Zones     : DE-LU (EIC 10Y1001A1001A82H), ES (EIC 10YES-REE------0)

DE-LU_weather.csv / ES_weather.csv
  Source    : Open-Meteo ERA5 reanalysis (https://open-meteo.com)
  Variables : temperature_2m, wind_speed_10m, wind_speed_100m,
              shortwave_radiation, direct_radiation, cloud_cover
  Frequency : hourly UTC
  Period    : 2022-01-01 to ~2 days before run date
  Coords    : DE-LU (51.5, 10.0), ES (40.4, -3.7)

DE-LU_generation.csv / ES_generation.csv
  Source    : ENTSO-E A75 (Actual Generation per Production Type)
  Variables : per-fuel MWh columns (wind, solar, nuclear, gas, hydro, etc.)
  Frequency : hourly UTC
  Period    : 2022-01-01 to ~2 days before run date

TTF gas and ETS carbon prices are interpolated from monthly reference values
(IEA Gas Market Report, Ember European Power Sector Review, Eurostat).
Place data/ttf_gas.csv or data/ets_carbon.csv (columns: Date, Price)
to use higher-resolution daily data from investing.com.
