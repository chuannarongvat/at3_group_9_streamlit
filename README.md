# AT3 Group 9 Streamlit Application

This repository contains the Streamlit application developed by AT3 Group 9.

## Getting Started
To run the Streamlit application locally, follow these steps:

1. Install the required dependencies using Poetry:
   ```shell
   poetry install
2. In the local directory, start the streamlit application:
    ```shell
    streamlit run streamlit/app.py

Project Organization
------------
    at3_group_9_streamlit/
    │
    ├── data/
    │ └── table.csv - Dataset containing relevant features.
    │
    ├── models/
    │ └── dt_regressor.joblib - The trained Decision Tree regressor model.
    │
    ├── streamlit/
    │ └── app.py - Streamlit application entry point.
    │
    ├── runtime.txt - Specifies the Python version for Streamlit Cloud.
    │
    ├── poetry.lock - Lock file ensuring reproducible builds.
    │
    └── pyproject.toml - Poetry file defining project dependencies and settings.

------------

