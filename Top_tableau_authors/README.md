# Title: "Top Tableau Experts with 10+ VOTD"

Programming:  Python 🐍.

🅰️ This repository contains the code and instructions for retrieving data for all Tableau Viz of the Day (VOTD) and visualizing the top authors using Tableau.

## Getting Started
To get started, you will need to have the following installed:

- Python 3
- Tableau Desktop

## Extracting Data using APIs (https://github.com/wjsutton/tableau_public_api).

- Retrieving VOTD Data (it contains only Viz Of The Day data).
- Get the list of Authors having at least 10 VOTD.
- Get all vizs for those authors.
- Get extra infor for each viz.
- Join all data for each authors having 10 or more VOTD and store it in a CSV file. 
- Connect the data source (CSV file) to the Tableau workbook.
- Visualize it using Tableau.

## Code: [Code](https://github.com/jigarpatel931/Python-Projects/blob/main/Top_tableau_authors/Top%20authors_tableau.ipynb)

## Tableau:
<a href="https://public.tableau.com/app/profile/jigarpatel136/viz/TopVizExperts10VOTD/Dashboard" target="_blank"><img align="center" src="https://github.com/jigarpatel931/Python-Projects/blob/main/Top_tableau_authors/Top_Authors_viz.png" alt="Tableau Report" height="200" width="300" /></a>



# Title: "Live VOTD Data extraction using API"

Programming:  Python 🐍.

🅰️ 2nd part: This project updates the VOTD (Viz of the Day) data on a Google Sheet using the Google Sheets API and Tableau's API. The code makes an API call to Tableau's gallery API to get the VOTD data and then updates the Google Sheet with the data. The code is designed to run on a regular schedule a task scheduler on schedule time. 

## Getting Started
To get started, you will need to have the following installed:

- Python 3
- Jupyter notebook
- Google Sheet/Drive API

## Steps

- Import necessary libraries including pandas, numpy, matplotlib, requests, schedule, time, croniter, json, urllib3, re, gspread, google.oauth2.credentials, oauth2client.service_account, and datetime.
- Set up authentication with the Google Sheets API using ServiceAccountCredentials.
- Open the Google Sheet to be updated and retrieve the URL of the first workbook from the sheet.
- Make an API call to Tableau's gallery API to get the VOTD data and append it to a list.
- Check if the first workbook URL is in the list of VOTD data. If it is not, insert all the data into the Google Sheet. If it is, insert only the new data into the Google Sheet.
- Convert the data to a list of lists and insert it into the Google Sheet.
- Append a log row to the Update_Log worksheet in the Google Sheet to record the timestamp and number of rows inserted.

## Code: [Code](https://github.com/jigarpatel931/Python-Projects/blob/main/Top_tableau_authors/VOTD_authors.ipynb)

## Google sheet: 
<a href="https://docs.google.com/spreadsheets/d/1YOOTbdN5lnGSVLf2c7H_Lfz6GxqGXXQRQUwtFJbLg4A/edit#gid=0" target="_blank"><img align="center" src="https://github.com/jigarpatel931/Python-Projects/blob/main/Top_tableau_authors/google%20sheet.PNG" alt="Tableau Report" height="200" width="300" /></a>
