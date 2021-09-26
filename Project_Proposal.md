![TLC logo](https://user-images.githubusercontent.com/87195262/134807871-6389592c-65f6-4fda-81be-86e3923bf1d9.png)
### Company info
The New York City Taxi and Limousine Commission (TLC) is an agency that is responsible for licensing and regulating New York City's taxi cabs. Over 200,000 TLC licensees complete approximately 1,000,000 trips each day.

### Problem statement
For the last four years, TLC has been working on making 50000 self-driving taxis to start distributing them in late 2021. They are planning to start by distributing the taxis at the subway stations. Therefore, they need to decide the distribution plan based on the number of units per station and the total number of exits per station.

### Value to the company
* Increase the availability of self-driving taxis at the most crowded stations.
* Reduce the number of redundant self-driving taxis at the least crowded stations.

### Data Description
The data that will be used in taking insights about the nature of subway stations congestion, and the number of exits registered per unit per station in New York City, is Metropolitan Transportation Authority (MTA). The dataset is downloaded from the MTA website that provides a series of data files containing numbers of cumulative entries and exits by stations, turnstile, along with their dates and time. The metro data records are weekly produced and mostly collected every 4 hours.
The dataset includes 11 columns and the following is the description of each feature:

| Field Name | Description                                                                     |
|------------|---------------------------------------------------------------------------------|
| C/A        | Control Area (A002)                                                             |
| UNIT       | Remote Unit for a station (R051)                                                |
| SCP        | Subunit Channel Position represents an specific address for a device (02-00-00) |
| STATION    | Represents the station name the device is located at                            |
| LINENAME   | Represents all train lines that can be boarded at this station                  |
| DIVISION   | Represents the Line originally the station belonged to BMT, IRT, or IND         |
| DATE       | Represents the date (MM-DD-YY)                                                  |
| TIME       | Represents the time (hh:mm:ss) for a scheduled audit event                      |
| DESC       | Represent the "REGULAR" scheduled audit event (Normally occurs every 4 hours)   |
| ENTRIES    | The comulative entry register value for a device                                |
| EXITS      | The cumulative exit register value for a device                                 |

### Scope
The scope of this project will be tested on the last three months of 2019 since the distribution plan will be started at the end of 2021. The data of 2020 is ignored since it might be affected by the Covid-19 pandemic.

### Tools
* Technologies: SQL, SQLite, Python, Jupyter notebook.
* Libraries: NumPy, Pandas, Matplotlib, Seaborn, SQLAlchemy.
