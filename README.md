# CTA Database Application

**Author:** Rahin Jain  
**Course:** CS 341 (Fall 2024)  
**Project:** CTA Database App  

## Description

The **CTA Database App** is an interactive Python-based application designed to analyze and explore data from the Chicago Transit Authority (CTA) using SQLite. This application provides insights into CTA's public transit system through queries, data visualizations, and interactive commands.

---

## Features

1. **General Statistics**  
   Retrieve basic statistics such as the total number of stations, stops, ridership entries, and data range.

2. **Search Station by Name**  
   Query stations by partial names using wildcards and view station IDs.

3. **Ridership Analysis by Station**  
   Analyze weekday, Saturday, and Sunday/holiday ridership statistics for a specific station.

4. **Weekday Ridership Rankings**  
   Display weekday ridership for all stations in descending order along with their percentage contribution.

5. **Stops by Line and Direction**  
   View stops along a specified train line and direction. Check accessibility information for each stop.

6. **Yearly Ridership Trends**  
   Display and optionally plot yearly ridership trends for a selected station.

7. **Monthly Ridership Trends**  
   Display and optionally plot monthly ridership trends for a selected station in a given year.

8. **Station Comparison**  
   Compare daily ridership between two stations for a given year and visualize the comparison.

9. **Stations Within One Mile**  
   Find all stations within a one-mile radius of given latitude and longitude coordinates. Includes optional plotting on a map.

---

## Requirements

- Python 3.x
- SQLite3
- matplotlib
- CTA Database (`CTA2_L_daily_ridership.db`)
- Chicago map image file (`chicago.png`)

---

## Installation

1. Ensure Python and SQLite3 are installed on your system.
2. Install required Python libraries:
   ```bash
   pip install matplotlib
   ```
3. Place the database file (`CTA2_L_daily_ridership.db`) and Chicago map image (`chicago.png`) in the same directory as `main.py`.

---

## Usage

1. Run the script:
   ```bash
   python main.py
   ```
2. Follow the on-screen instructions to input commands and interact with the app.

### Commands

| Command | Description                                 |
|---------|---------------------------------------------|
| 1       | Search station by partial name.            |
| 2       | Analyze ridership statistics for a station.|
| 3       | View weekday ridership rankings.           |
| 4       | List stops by train line and direction.    |
| 5       | Show stop counts and percentages by line.  |
| 6       | View and plot yearly ridership trends.     |
| 7       | View and plot monthly ridership trends.    |
| 8       | Compare daily ridership between two stations.|
| 9       | Find stations within a one-mile radius.    |
| x       | Exit the application.                      |

---

## File Structure

- `main.py`: Main script for the application.
- `CTA2_L_daily_ridership.db`: SQLite database file containing CTA data.
- `chicago.png`: Map image for plotting nearby stations.

---

## Example Usage

1. Start the app and view general statistics.
2. Search for a station using its partial name (Command 1).
3. Analyze the ridership of a specific station (Command 2).
4. Compare ridership trends between two stations (Command 8).
5. Visualize yearly or monthly ridership trends (Commands 6 & 7).

---

## Notes

- Ensure the database file and image are in the correct directory for full functionality.
- Input formats for commands are case-insensitive (e.g., "Red" and "red" are treated the same).
