# NewsUnravel: Creating a Media Bias Indicating and Feedback Collecting News-Reading Application

## Introduction

This repository contains all code and resources from the paper "NewsUnravel: Creating a Media Bias Indicating and Feedback Collecting News-Reading Application".
The paper can be found on 
TODO

## Directories

The two distinct applications are separated into the following two directories.
Further instructions and information can be found in the respective README.md files.

- `feedback-mechanism-study`: contains the code, data and evaluation notebooks of the Feedback Mechanism Study.
- `newsunravel-platform`: contains the code, data and evaluation notebooks of the NewsUnravel Platform.

## Local Development

To develop locally you have to configure and run a database and two applications:

### Database

Run a PostgreSQL database using your preferred method (bare metal, Docker etc).

### Inference API

First, configure and start the Inference API:

- Install Python >=3.10
- Install poetry: `pip install poetry`
- Install dependencies: `poetry install`
- Configure the environment variables by copying the `apps/inference/.env.example` file to `apps/inference/.env`
- Run `poetry run prepare`
- Run the app using `poetry run inference`

### Platform

Then, configure and start the Platform:

- Install NodeJS >= 16
- Install yarn: `npm i -g yarn`
- Install dependencies using `yarn install`
- Configure the environment variables by copying the `apps/inference/.env.example` file to `apps/inference/.env` and adjusting the values
- Run the app using `yarn run dev`

## Training and Evaluation

Run the Jupyter notebooks in the respective `evaluation/` subdirectories with an R oder Python 3 kernel (depending on the content).

## Citation

Please cite us as:

TODO