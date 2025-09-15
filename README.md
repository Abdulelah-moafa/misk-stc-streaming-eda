# Misk × STC — Streaming EDA (Virtual Work Experience)

This repo contains my **Data Cleaning** and **Descriptive Statistics** work completed as part of a **Virtual Work Experience via Misk in collaboration with STC**.

## Dataset
- Size: **1,048,575 rows × 13 columns**
- Sample columns: `date_`, `user_id_maped`, `program_name`, `duration_seconds`, `program_class`, `season`, `episode`, `program_genre`, `hd`, ...
- Raw data lives in `data/raw/` (tracked via **Git LFS** or shared via **Releases**). A small sample is in `data/sample/`.

## What I did
- Load `.xlsb` with `pyxlsb`; sheet = `Final_Dataset`
- Clean text fields & convert `date_ → watch_date`
- Derive `duration_min`; map `hd → HD/SD`
- Handle missing values (Median/Mode) & drop exact duplicates
- Compute numeric **mean / std / min / max** (`agg`) for: `duration_seconds`, `duration_min`, `season`, `episode`, `hd`

