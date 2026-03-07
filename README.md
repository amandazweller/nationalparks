# National Park Recreation Dataset

This repository contains the code and dataset for a data curation project completed for **STAT 386**. The goal of this project was to create an original dataset using an API and Python, then document the process of collecting and preparing the data.

The dataset was created using the developer API from the National Park Service. It contains information about park characteristics, location, and recreational opportunities across parks managed by the National Park Service.

---

## Project Overview

The purpose of this project was to build a dataset that could be used to explore patterns in recreation opportunities across U.S. national parks. In particular, the dataset includes information about whether parks offer activities such as camping, fishing, and wildlife-related experiences.

The data was collected using the National Park Service API and processed using Python.

Example questions that could be explored with this dataset include:

- How common are camping and fishing opportunities across parks?
- Do certain park types offer more recreational activities than others?
- How do activity offerings vary across different parks?

---

## Data Source

Data for this project was obtained from the official developer API provided by the National Park Service.

National Park Service Developer API:  
https://www.nps.gov/subjects/developer/index.htm

The API provides structured information about parks managed by the National Park Service, including activities, topics, geographic coordinates, and other metadata.

---

## Repository Contents
```
national-parks-data/
│
├── get_parks_data.py
├── national_parks_dataset.csv
├── README.md
├── .env.example
└── .gitignore
```


### Files

**scrapedata.ipynb**

Jupyter notebook used to collect the data from the National Park Service API. The script sends a request to the parks endpoint, extracts selected fields, and saves the resulting dataset as a CSV file.

**national_parks_dataset.csv**

The final curated dataset used for the project.

**.gitignore**

Ensures that sensitive files such as `.env` are not included in the repository.

---

## Dataset Description

The dataset contains information about parks managed by the National Park Service.

Each row represents a single park unit.

### Dataset Size

- Approximately **400 parks**
- **15 features**

### Data Dictionary

| Feature | Description |
|-------|-------------|
| park_name | Full name of the park |
| park_code | Unique park identifier |
| states | State(s) where the park is located |
| designation | Type of park (National Park, Monument, Historic Site, etc.) |
| latitude | Geographic latitude |
| longitude | Geographic longitude |
| num_activities | Number of activities listed for the park |
| num_topics | Number of topics associated with the park |
| num_entrance_fees | Number of entrance fee options |
| description_length | Length of the park description |
| has_camping | Whether camping is available |
| has_fishing | Whether fishing is available |
| has_wildlife | Whether wildlife-related activities are present |
| has_biking | Whether biking is available |
| has_boating | Whether boating is available |

---

