
# SpaceX Launch Data Collection and Cleaning

## Overview

We will collect and clean SpaceX launch data using their REST API and some web scraping. The goal is to create a clean dataset to predict if SpaceX will try to land the rocket’s first stage.

---

## Steps

1. **Get Launch Data from API**

   * Use the endpoint: `https://api.spacexdata.com/v4/launches/past`
   * Make a GET request and get JSON data.

2. **Convert JSON to DataFrame**

   * Use `json_normalize()` to turn the JSON into a table.

3. **Web Scrape Falcon 9 Launch Tables**

   * Use BeautifulSoup to scrape launch data from Wikipedia pages.

4. **Clean and Prepare Data**

   * Filter out Falcon 1 launches, keep only Falcon 9.
   * Handle missing values in important columns like PayloadMass by filling with the mean.
   * Leave some missing values like LandingPad for later handling.
   * Use other API endpoints to get details for IDs in the data.

