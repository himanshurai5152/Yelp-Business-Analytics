# Yelp Data Analytics Project

## Overview

This workspace contains a Yelp academic dataset and a Jupyter notebook for data analytics using SQLite and Python.

The main notebook is:
- `SQL PROJECT for data analytics TECH CLASSES.ipynb`

It loads Yelp JSON datasets into pandas DataFrames, converts them to SQLite tables, and performs exploratory data analysis.

## Datasets

The available Yelp JSON files are:
- `yelp_academic_dataset_business.json`
- `yelp_academic_dataset_checkin.json`
- `yelp_academic_dataset_review.json`
- `yelp_academic_dataset_tip.json`
- `yelp_academic_dataset_user.json`

These files are line-delimited JSON and can be loaded incrementally to avoid memory issues.

## Project Goals

The notebook includes a problem statement and research objectives focused on:
- analyzing user engagement (reviews, tips, check-ins)
- evaluating relationships with business success metrics such as review counts and star ratings
- exploring sentiment and temporal trends in Yelp data

## How to run

1. Open `SQL PROJECT for data analytics TECH CLASSES.ipynb` in Jupyter or VS Code.
2. Ensure the notebook's dataset file paths point to the local `H:\Yelp_data` folder.
3. Run the notebook cells in order.

The notebook creates a local SQLite database file named `yelp.db` and loads the following tables:
- `business`
- `review`
- `user`
- `tip`
- `checkin`

## Key steps in the notebook

- Load each JSON dataset into pandas DataFrames
- Clean and type-convert the data
- Save DataFrames to a SQLite database
- Connect to `yelp.db` and inspect table contents
- Run SQL-based exploratory analysis on restaurant data

## Notes

- The notebook currently reads the first 50,000 lines from each JSON dataset for initial analysis.
- If you want to load the full dataset, adjust the `islice` limits or remove them.

## License

This repository contains publicly available Yelp academic dataset files for learning and analytics purposes.
