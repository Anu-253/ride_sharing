# Ride-Sharing ETL Pipeline

A data engineering case study that processes ride-sharing data using PySpark, HDFS, and PostgreSQL.

## Project Overview

Ride-sharing applications generate large amounts of trip data. This project aims to build an ETL (Extract, Transform, Load) pipeline to process ride records, calculate trip duration, validate data, calculate driver payouts, and store verified results in PostgreSQL.

## Objectives

- Extract ride data from a Kaggle dataset.
- Process and transform data using PySpark.
- Calculate trip duration and validate ride records.
- Store ride telemetry in JSON format using HDFS.
- Apply driver payout tiers and surge multiplier rules.
- Log invalid records for error handling.
- Load verified payout records into PostgreSQL.

## Dataset

**Source:** [Uber Trips Dataset — Kaggle](https://www.kaggle.com/datasets/rohiteng/uber-trips-dataset)

The dataset contains approximately 50,000 ride records, including driver IDs, pickup and drop-off coordinates, trip distance, fare amount, ride status, payment method, and timestamps.

## Technology Stack

- Python
- PySpark
- HDFS
- PostgreSQL
- Google Colab
- Kaggle

## ETL Workflow

1. **Extract:** Download and load the Kaggle CSV dataset.
2. **Transform:** Calculate trip duration and validate ride records.
3. **Store:** Prepare ride telemetry in JSON format for HDFS.
4. **Calculate:** Apply documented payout-tier and surge rules.
5. **Validate:** Separate invalid records and record error reasons.
6. **Load:** Store verified payout records in PostgreSQL.

## Project Status

🚧 In progress — data loading and initial transformations are being implemented.

## Expected Outcomes

- Processed ride records with calculated trip durations.
- Validation and error logs.
- Driver payout calculations.
- JSON ride telemetry.
- Verified payout records in PostgreSQL.

## Disclaimer

Surge multipliers and payout tiers will be defined as separate project business rules because they are not directly supplied by the source dataset.

## Author

Anagha P. Kulkarni
