# SeaWatch Plane Tracking Project

This repository contains information and guidelines for the SeaWatch team's project aimed at tracking active planes in the central Mediterranean region.

## Project Overview

SeaWatch aims to monitor plane activities in the central Mediterranean, particularly focusing on identifying Frontex activities and ensuring compliance with search patterns and rescue operations rather than pushbacks.

## Objectives

1. **Data Gathering**: Utilize ADSB (Automatic Dependent Surveillance-Broadcast) data from [ADSB Exchange](https://www.adsbexchange.com/) to gather information on plane activities, excluding military and state actors.
2. **Historical Data Analysis**: Gather historical data for reconstruction purposes, analyzing past incidents and potential involvement in pushback situations.

3. **Database Management**: Establish a PostgreSQL database to store flight data spanning the last 3-4 years continuously.

4. **Real-time Monitoring**: Develop a system to monitor live flight patterns, identifying deviations from standard search patterns or distress situations.

## Key Information

- **ADSB Exchange API**: Consider reaching out to ADSB Exchange for data access, but be prepared to build a scraper due to potential limitations and costs associated with the API.

- **Flight Characteristics**: Understand typical flight patterns and durations to differentiate between routine patrols, distress situations, and search and rescue operations.

- **Frontex Search Patterns**: Refer to [Marine Teacher](https://www.marineteacher.com/post/iamsar-search-patterns) for insights into Frontex's search patterns.

- **Communication Protocols**: Ensure timely communication with SeaWatch, ideally providing updates within 5-10 minutes of any relevant flight pattern deviations.

## First Steps

1. **Acquire Aircraft List**: Obtain a list of aircraft of interest from Tassilo, possibly including ADSB hex codes for identification purposes.

2. **Data Access**: Contact ADSB Exchange for potential data access. If not feasible, prepare to build a data scraper for live data collection.

3. **Database Structure**: Design and implement a suitable PostgreSQL database structure to accommodate the collected flight data.

4. **Pipeline Setup**: Establish an automated pipeline for data collection, processing, and analysis.

## Set up

### PIP requirements

- to export:
  ip freeze > requirements.txt

- to install:
  pip install -r requirements.txt
