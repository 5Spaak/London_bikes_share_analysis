## Analysis On London Bikes Share

### Description of dataset

The data from cycling dataset is grouped by "Start time", this represent the count of new bike shares grouped by hour. The long duration shares are not taken in the count. You can find the dataset here [link](https://www.kaggle.com/datasets/hmavrodiev/london-bike-sharing-dataset?rvi=1)

There are several files in this projet :

- london_bikes_final.csv: the final file after analysis and cleaning
- london_merged.csv: the started file for analysis
- london_bikes.ipynb: The file that contains our analysis
- london-bike-sharing.zip : The file download with a helper library opendataset
- README.md : This files contains information about dataset !

### Context or goal of the projet

The purpose is to analyse and explore the dataset before use Tableau Desktop for visualization. This is the first version of the projet. Here we only have a Exploratory Data Analysis

### Metadata:

- "timestamp" - timestamp field for grouping the data
- "cnt" - the count of a new bike shares
- "t1" - real temperature in C
- "t2" - temperature in C "feels like"
- "hum" - humidity in percentage
- "wind_speed" - wind speed in km/h
- "weather_code" - category of the weather
- "is_holiday" - boolean field - 1 holiday / 0 non holiday
- "is_weekend" - boolean field - 1 if the day is weekend
- "season" - category field meteorological seasons: 0-spring ; 1-summer; 2-fall; 3-winter.

"weathe_code" category description:

1. = Clear ; mostly clear but have some values with haze/fog/patches of fog/ fog in vicinity
2. = scattered clouds / few clouds
3. = Broken clouds
4. = Cloudy
5. = Rain/ light Rain shower/ Light rain
6. = rain with thunderstorm
7. = snowfall
8. = Freezing Fog

## Columns rename

- **'timestamp'**: 'time',
- **'cnt'** : 'count',
- **'t1'**:'temp_real_celcius',
- **'t2'**:'temp_feels_like',
- **'hum'**:"humidity",
- **'wind_speed'**:'wind_speed_kph',
- **'weather_code'**:'weather',
- **'is_holiday'**:'is_holiday',
- **'is_weekend'**:'is_weedend',
- **'season'**:'season'

## season column rename

- **'0.0'**:'spring',
- **'1.0'**:'summer',
- **'2.0'**:'autumn',
- **'3.0'**:'winter'

## weather column rename

- **"1.0"**: 'Clear',
- **"2.0"**:'Scattered clouds',
- **"3.0"**:'Broken clouds',
- **"4.0"**: 'Cloudy',
- **"7.0"**:'Rain',
- **"10.0"**:'Rain with thunderstorm',
- **"26.0"**:'Snowfall'
