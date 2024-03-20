# nosql-challenge

## Overview
In this project, I analyze food hygiene ratings data from the UK Food Standards Agency. The analysis explores the hygiene scores, business types, and geographical distribution of food establishments to identify trends and insights.


### Prerequisites
- MongoDB (and MongoDB tools)
- Python 3
- Jupyter Notebook
- Libraries: PyMongo, pprint, pandas

## Part 1: Database and Jupyter Notebook Setup
**Data Import**: I used the `establishments.json` file to import data into MongoDB. I used the following command in my Terminal, after first navigating to where my `establishments.json` file is located in bash:

```bash
mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
```
## Part 2: Update Database
I then updated the database, inserting a new document and changing several fields from string to integer for the entire collection.

## Part 3: Exploratory Analysis
I analyzed the following questions within my exploratory analysis: 
1. Identified establishments with a hygiene score of 20.
2. Found establishments in London with a RatingValue greater than or equal to 4.
3. Determined the top 5 establishments with a RatingValue of 5, sorted by the lowest hygiene score and proximity to "Penang Flavours".
4. Counted how many establishments in each Local Authority area have a hygiene score of 0, sorting the results from highest to lowest.

