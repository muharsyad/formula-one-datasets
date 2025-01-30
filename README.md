# Formula One Dataset

This repository contains a collection of Formula One datasets sourced from [Ergast Developer API](https://ergast.com/mrd/). The datasets provide detailed information about various aspects of Formula One racing, including circuits, drivers, constructors, lap times, pit stops, qualifying results, race results, races, seasons, sprint results, and status.

## Datasets

The repository includes the following CSV files:

1. **circuits.csv**  
   - **Description**: Information about the circuits where Formula One races are held.
   - **Columns**:
     - `circuitId`: Unique identifier for the circuit.
     - `circuitName`: Name of the circuit.
     - `lat`: Latitude of the circuit location.
     - `long`: Longitude of the circuit location.
     - `locality`: Locality or city where the circuit is located.
     - `country`: Country where the circuit is located.
     - `url`: URL with more information about the circuit.

2. **constructors.csv**  
   - **Description**: Information about the constructors (teams) participating in Formula One.
   - **Columns**:
     - `constructorId`: Unique identifier for the constructor.
     - `constructorName`: Name of the constructor.
     - `nationality`: Nationality of the constructor.
     - `url`: URL with more information about the constructor.

3. **drivers.csv**  
   - **Description**: Information about the drivers participating in Formula One.
   - **Columns**:
     - `driverId`: Unique identifier for the driver.
     - `givenName`: Given name of the driver.
     - `familyName`: Family name of the driver.
     - `code`: Driver's abbreviation code.
     - `permanentNumber`: Permanent number assigned to the driver.
     - `dateOfBirth`: Date of birth of the driver.
     - `nationality`: Nationality of the driver.
     - `url`: URL with more information about the driver.

4. **lap_times.csv**  
   - **Description**: Lap times for drivers during races.
   - **Columns**:
     - `season`: Season year.
     - `round`: Round number in the season.
     - `lapNumber`: Lap number.
     - `driverId`: Unique identifier for the driver.
     - `position`: Position of the driver at the end of the lap.
     - `time`: Time taken to complete the lap.

5. **pitstops.csv**  
   - **Description**: Information about pit stops during races.
   - **Columns**:
     - `season`: Season year.
     - `round`: Round number in the season.
     - `driverId`: Unique identifier for the driver.
     - `lap`: Lap number when the pit stop occurred.
     - `stop`: Stop number during the race.
     - `time`: Time when the pit stop occurred.
     - `duration`: Duration of the pit stop.

6. **qualifying_results.csv**  
   - **Description**: Results of qualifying sessions.
   - **Columns**:
     - `season`: Season year.
     - `round`: Round number in the season.
     - `driverId`: Unique identifier for the driver.
     - `driverName`: Name of the driver.
     - `constructorId`: Unique identifier for the constructor.
     - `constructorName`: Name of the constructor.
     - `number`: Car number.
     - `position`: Position in the qualifying session.
     - `q1`: Time in Q1.
     - `q2`: Time in Q2.
     - `q3`: Time in Q3.

7. **race_results.csv**  
   - **Description**: Results of races.
   - **Columns**:
     - `season`: Season year.
     - `round`: Round number in the season.
     - `driverId`: Unique identifier for the driver.
     - `driverName`: Name of the driver.
     - `constructorId`: Unique identifier for the constructor.
     - `constructorName`: Name of the constructor.
     - `number`: Car number.
     - `position`: Finishing position.
     - `positionText`: Finishing position as text.
     - `points`: Points earned.
     - `grid`: Starting grid position.
     - `laps`: Number of laps completed.
     - `status`: Status at the end of the race.
     - `time`: Total race time.
     - `fastestLapRank`: Rank of the fastest lap.
     - `fastestLap_lap`: Lap number of the fastest lap.
     - `fastestLapTime`: Time of the fastest lap.
     - `averageSpeed`: Average speed during the race.

8. **races.csv**  
   - **Description**: Information about the races.
   - **Columns**:
     - `season`: Season year.
     - `round`: Round number in the season.
     - `raceName`: Name of the race.
     - `circuitId`: Unique identifier for the circuit.
     - `circuitName`: Name of the circuit.
     - `date`: Date of the race.
     - `time`: Time of the race.
     - `firstPractice`: Date and time of the first practice session.
     - `secondPractice`: Date and time of the second practice session.
     - `thirdPractice`: Date and time of the third practice session.
     - `qualifying`: Date and time of the qualifying session.
     - `sprint`: Date and time of the sprint race (if applicable).
     - `url`: URL with more information about the race.

9. **seasons.csv**  
   - **Description**: Information about the seasons.
   - **Columns**:
     - `season`: Season year.
     - `url`: URL with more information about the season.

10. **sprint_results.csv**  
    - **Description**: Results of sprint races.
    - **Columns**:
      - `season`: Season year.
      - `round`: Round number in the season.
      - `driverId`: Unique identifier for the driver.
      - `driverName`: Name of the driver.
      - `constructorId`: Unique identifier for the constructor.
      - `constructorName`: Name of the constructor.
      - `number`: Car number.
      - `position`: Finishing position.
      - `positionText`: Finishing position as text.
      - `points`: Points earned.
      - `grid`: Starting grid position.
      - `laps`: Number of laps completed.
      - `status`: Status at the end of the sprint race.
      - `time`: Total sprint race time.
      - `fastestLap_lap`: Lap number of the fastest lap.
      - `fastestLapTime`: Time of the fastest lap.

11. **status.csv**  
    - **Description**: Status information.
    - **Columns**:
      - `statusId`: Unique identifier for the status.
      - `status`: Description of the status.
      - `count`: Number of occurrences of the status.

## Usage

- To use these datasets, simply clone the repository and load the CSV files into your preferred data analysis tool (e.g., Python with pandas, R, Excel, etc.).

```bash
git clone https://github.com/muharsyad/formula-one-datasets.git
```
- The dataset can be used for various Formula 1 data analysis tasks, including race predictions, performance analysis, and statistical insights.
- Each CSV file can be loaded into Python using pandas:
  ```python
  import pandas as pd
  df = pd.read_csv('race_results.csv')
  print(df.head())
  ```

## License

This dataset is provided for educational and analytical purposes. Please check the [Ergast API terms of use](https://ergast.com/mrd/terms/) before using the data for commercial purposes.

## Acknowledgments

- [Ergast Developer API](https://ergast.com/mrd/) for providing the Formula One data.
- Formula One Management for the original data.

## Contact

For any questions or suggestions, please open an issue in this repository or contact me directly.



