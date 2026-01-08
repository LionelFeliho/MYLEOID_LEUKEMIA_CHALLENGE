# QRT_PROJECT

Baseline work for the Challenge Data ENS myeloid leukemia risk prediction competition.
This repository contains a benchmark notebook that explores survival analysis on the
challenge-provided clinical and molecular datasets.

## Project overview

The goal of the challenge is to predict overall survival (time-to-event with censoring)
for adult myeloid leukemia patients using clinical measurements and somatic mutation data.
The provided data includes patient-level clinical features, survival outcomes for training
patients, and per-mutation molecular records that can be aggregated into modeling features.

## What this repo does

The `Benchmark_nqBJ7fO.ipynb` notebook walks through:

- Preparing the clinical training data for survival analysis (OS_YEARS, OS_STATUS).
- Building a baseline LightGBM regression model that ignores censoring.
- Training a Cox proportional hazards model that accounts for censoring.
- Adding a simple mutation burden feature by counting mutations per patient.
- Running inference for the test set to produce predictions.

## Challenge link

- https://challengedata.ens.fr/participants/challenges/162/
