# London Bike Rides Dashboard and Data Cleaning Project

## Overview
This project focuses on analyzing and visualizing data related to bike rides in London. The dataset spans from January 2015 to January 2017 and includes metrics such as temperature, wind speed, and ride counts. The dashboard and data cleaning process were implemented using Tableau and Python, respectively.

## Dashboard
The interactive dashboard, published using Tableau, provides insights into:
- **Total bike rides**: 19,359,333 rides January 2015 to January 2017.
- **Temperature vs. Wind Speed**: A heatmap comparing the distribution of bike rides across varying temperatures and wind speeds.
- **Trends over time**: A line graph showing ride trends across the timeline, with a moving average feature for better trend analysis.

### Key Features
- Dynamic filters for exploring specific time periods.
- Dynamic adjustments for exploring the impact of difference moving average on the trend line.
- Clear visualization of the impact of weather conditions on bike rides.
- Intuitive interface for analyzing large datasets.

## Data Cleaning
The data cleaning process was performed using Python in a Jupyter Notebook. Below are the key steps:

### Tools Used
- **Python**: For data cleaning and preprocessing.
- **Pandas**: To manipulate and analyze the dataset.
- **Jupyter Notebook**: For an interactive coding environment.

### Steps
1. **Unzipping the Dataset**:
   ```python
   zipfile_name = 'london-bike-sharing-dataset.zip'
   with zipfile.ZipFile(zipfile_name, 'r') as file:
       file.extractall()
   ```

2. **Reading the CSV File**:
   ```python
   bikes = pd.read_csv('london_merged.csv')
   ```

3. **Exploring the Data**:
   - Displaying the first few rows:
     ```python
     bikes.head()
     ```
   - Checking the dataset shape:
     ```python
     bikes.shape
     ```

4. **Counting Unique Values in a Column**:
   ```python
   bikes.weather_code.value_counts()
   ```

## File Structure
- `london-bike-sharing-dataset.zip`: Raw dataset.
- `london_merged.csv`: Unzipped dataset used for analysis.
- `london_bikes_final.xlsx`: Processed data for dashboard.
- `london_bikes.ipynb`: Python notebook for data cleaning.

## How to Use
1. **Run the Jupyter Notebook**:
   - Ensure you have Python and Jupyter Notebook installed.
   - Open `london_bikes.ipynb` and run the cells sequentially.

2. **View the Dashboard**:
   - Access the published Tableau dashboard for interactive analysis.
   

## Requirements
- Python 3.8+
- Libraries: `pandas`, `zipfile`
- Tableau Public or Tableau Desktop for dashboard visualization.


## Author
Hoangky Nguyen
