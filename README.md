# Practical Work No. 1 - Introduction to Data Analytics and Google Colab

This repository contains my solution for Practical Work No. 1. The goal of the work is to learn how to create notebooks in the cloud-based Google Colab environment, load and explore tabular data with **Pandas**, and perform basic vectorised computations with **NumPy**.

## Repository contents

| File | Description |
|------|-------------|
| `karpiuk_lab.ipynb` | Practical part (Steps 1-7): importing libraries, mounting Google Drive, reading a CSV file into a DataFrame, initial data inspection, and basic NumPy array operations. |
| `Пр_1_Аналітики.ipynb` | Individual tasks 1-7 and the additional ★ task: library versions, `head()` / `tail()`, `df.columns`, 1D and 2D NumPy arrays, Markdown cells, reading data from Google Drive, and a combined analysis notebook. |
| `README.md` | This file. |

## Dataset

The notebooks use `sales.csv` - a coffee shop transactions dataset with the following columns:

| Column | Description |
|--------|-------------|
| `date` | Transaction date |
| `datetime` | Transaction date and time |
| `cash_type` | Payment type (`card` / `cash`) |
| `card` | Anonymised card identifier (empty for cash payments) |
| `money` | Transaction amount |
| `coffee_name` | Name of the drink |

If `sales.csv` is not found on Google Drive, the notebooks automatically generate a small synthetic sample with the same structure (60 rows), so every cell can be run without extra preparation.

## How to run

1. Open [Google Colab](https://colab.research.google.com) and sign in with your Google account.
2. Choose **File → Upload notebook** and select one of the `.ipynb` files (or open it directly from GitHub).
3. Upload `sales.csv` to the root of your Google Drive (`MyDrive`), or skip this step to use the generated sample.
4. Run the cells in order with **Shift + Enter**. When prompted by `drive.mount('/content/drive')`, grant access to your Drive.

> Note: the Drive mount is valid only for the current session and must be repeated after the runtime restarts.

## Requirements

- Python 3 (pre-installed in Google Colab)
- `pandas`
- `numpy`

Both libraries are pre-installed in Colab, so no additional setup is needed.

## What was covered

- Creating and naming a Colab notebook; code and text cells
- Importing `pandas as pd` and `numpy as np`
- Mounting Google Drive and reading files with `pd.read_csv()`
- Initial data exploration: `head()`, `tail()`, `shape`, `info()`, `describe()`, `columns`
- NumPy arrays: creation, `dtype`, `shape`, element-wise arithmetic (vectorisation), aggregate functions (`sum`, `mean`, `min`, `max`) and the `axis` parameter
- Documenting work with Markdown cells

## Author

Karpiuk
