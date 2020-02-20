## A four stage roadmap

There are 4 phases to the scraping approach:

* 1st phase - We can scrape
* 2nd phase - We can scrape sustainably & technical debugging of crashes
* 3rd phase -  Ed can CRUD harvesters/scrappers & non-technical debugging of crashes
* 4th phase - Move away from scraping and towards structured data-pipeline based on a data strategy

### 1st phase - Scraping

To scrape the Dept Ed websites and use data wrangling to populate the ODP with metadata (and maybe data). This will start with a 2-week sprint to validate that this approach will likely meet the coverage and metadata quality objectives. 

The scraping / data wrangling output will be a data.json that will be ingested by a legacy Harvester. 

This will be a one-off process to support the launch of the catalog with as much coverage as possible. 

It will start with a 3 week test (1 week to prepare for a sprint, 2 week sprint) - at the end of this we will decide whether the scrapping approach is a viable option to populate the catalog

### 2nd phase - Scrape sustainably

To build on the above so that:
* Can be run at intervals or on-demand by developer
* Before loading in data into the portal, check for diff
* Scraping pipeline works with data.json "aka proper" pipeline (no duplication and Harvester favors the data.json ww2 file over web scrapping) 

This will probably involve using the NG Harvester pipeline, ie the backend NG Harvester infra but none of the front-end customization. 

### 3rd phase - CRUD harvesters/scrappers

NG Harvester
