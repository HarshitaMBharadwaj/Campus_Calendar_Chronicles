# GWU Events Scraper Challenge 📅

## Overview
This project involves scraping event information from the George Washington University (GWU) events calendar webpage and displaying various details about each event. The extracted information includes event titles, date information, locations, images, and primary event types. Additionally, the script converts the extracted data into a pandas DataFrame, performs data exploration and analysis, and exports the results to a CSV file.

## Instructions
1. The script requests the HTML page contents of the GWU events calendar.
2. It parses the page and loops through the events to display relevant information about each event, including:
   - Title
   - Date information (date, day of the week, start time, and end time)
   - Location
   - Image (if available)
   - Primary event type
3. Bonus: The script further decomposes the date information into separate fields such as date, day of the week, start time, and end time.
4. The extracted event details are stored in a list of dictionaries called `events`.
5. The list of events is converted into a pandas DataFrame called `events_df`.
6. The script provides summary information about the DataFrame, including column names, the number of rows, and the first few rows.
7. It also prints the earliest start time and the latest end time from the DataFrame.
8. The DataFrame contents are written to a CSV file named "events.csv" in the Colab filesystem.

## Further Exploration
- The script includes a function called `fetch_events` that accepts a date string as input and returns the events occurring on that day.
- By default, if no date is provided, it returns the events for the current day.
- To use this function, specify a date string in the format "YYYY-MM-DD" as the parameter `selected_date`.

## How to Run
- Simply execute the provided Python script in a Python environment with the necessary dependencies installed (requests, BeautifulSoup, pandas).
- Ensure that the Python script has permission to access the GWU events calendar webpage.

