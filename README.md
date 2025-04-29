---
title: Homework 8 – World Bank Data Loader
format: html
---

# 📦 Homework 8 – World Bank Data Loader

This folder contains the code used to populate the **MySQL** server with data for **Homework Assignment 8** in **CMSC 408**.

Everything needed to set up the database is contained within **`loader.qmd`**.

---

# ⚙️ Overview of the Pipeline

The **`loader.qmd`** document performs the following steps:

1. **Downloads** source data in ZIP format from the World Bank Data Store.
2. **Unzips** the required CSV files needed for analysis.
3. **Loads** the extracted CSVs into **MySQL** using **Pandas** and **SQLAlchemy**.
4. **Sets permissions** for users to access the loaded tables.

By running `loader.qmd`, you will automatically fetch, clean, load, and configure the World Bank data for analysis.

---

# 🚀 How to Run

## Prerequisites

Ensure the following Python packages are installed:

- pandas
- sqlalchemy
- python-dotenv
- mysql-connector-python or equivalent MySQL client

You can install them with:

```bash
pip install pandas sqlalchemy python-dotenv mysql-connector-python
```

## Execution  
To run the full data loading pipeline:

quarto render loader.qmd
