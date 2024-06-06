# 📊 Event Scenario Finder

The "Event Scenario Finder" is a Python script designed to analyze event data sourced from a Google BigQuery dataset. 

<img align="right" alt="Coding" width="400" src="https://kondado.io/assets/images/source-bigquery.gif">

## Features
- **Data Extraction**: Fetches event data from a specified Google BigQuery dataset.
- **Data Transformation**: Normalizes the event data to facilitate analysis.
- **User Behavior Tracking**: Tracks user behavior by grouping events based on user pseudo IDs.
- **Event Scenario Identification**: Identifies specific event scenarios, such as the transition from a session start to the addition of payment information.

## Usage
1. Ensure you have the necessary dependencies installed: `google-cloud-bigquery`, `pandas`, `tabulate`, and `dotenv`.
2. Set up your Google Cloud credentials and environment variables as specified in the `.env` file.
3. Run the script to fetch and analyze the event data from the BigQuery dataset.
4. View the identified event scenarios in the output.

## How it Works
The script begins by connecting to Google BigQuery and executing a query to fetch event data from the specified dataset. It then normalizes the data for better analysis, extracting information such as device details and geographic location.

Next, it sorts the data based on user pseudo IDs and event timestamps to track user behavior over time. Finally, it identifies specific event scenarios by searching for sequences of events, such as the transition from a session start to the addition of payment information.

## Example Usage
