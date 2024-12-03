# Air Quality Data Pipeline and Dashboard

This project builds a complete data pipeline to extract, transform, and visualize air quality data. It integrates the **Open Air Quality API** as the data source, processes the data for storage in a **DuckDB database**, and visualizes the results through an interactive dashboard built with **Plotly Dash**.

## Project Structure

├── README.md # Project documentation<br>
├── requirements.txt # Dependencies<br>
├── main.py # Main script to run the ETL pipeline and dashboard<br>
├── extract.py # Handles data extraction from the Open Air Quality API<br>
├── transform.py # Contains data transformation logic<br>
├── load.py # Handles loading data into DuckDB<br>
├── dashboard.py # Dashboard implementation using Plotly Dash<br>
├── data/ # Directory for intermediate and raw data (if necessary)<br>
└── duckdb/ # Directory for DuckDB files


## Features

- **Extract:** Connects to the Open Air Quality API to retrieve air quality data.
- **Transform:** Cleans, filters, and structures the data for efficient analysis.
- **Load:** Stores the processed data in a DuckDB database for querying.
- **Visualize:** Provides an interactive dashboard to explore air quality trends.

## Getting Started

### Prerequisites

Ensure you have the following installed:

- Python 3.8+
- DuckDB

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/billobah/air_quality_dashboard.git
   cd air_quality_dashboard
   ```

2. Create a virtual environment for your project:
   ```bash
   python3 -m venv venv
   ```

3. Activate the virtual environment:

- On **Linux/macOS:**

  ```bash
  source venv/bin/activate
  ```

- On **Windows:**
 
  ```bash
  .\venv\Scripts\activate
  ``` 

This will create a folder named venv containing the virtual environment.

3. Install dependencies:
  ```bash
  pip install -r requirements.txt
  ```

### Running the Project

1. Run the ETL pipeline:
   ```bash
   python main.py
   ```

2. Open the dashboard: Navigate to http://127.0.0.1:8050 in your browser to explore the air quality data.

## File Details

```extract.py```
Contains logic to fetch data from the Open Air Quality API.

```transform.py```
Implements data cleaning and transformation steps.

```load.py```
Manages loading data into a DuckDB database.

```dashboard.py```
Creates a Plotly Dash dashboard for visualizing air quality trends.

## Future Enhancements
- Add support for real-time data updates.
- Integrate with more APIs for broader data coverage.
- Enhance dashboard visualizations.