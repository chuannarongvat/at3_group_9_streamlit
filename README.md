# Advanced Machine Learning Assignment 3: Group 9 Streamlit Application

This repository contains the Streamlit application developed by AT3 Group 9.

**Links to the Streamlit application (click to access):**  
## [Streamlit Application](https://at3group9app-j9uwhfpnn3xj8jxffdkedh.streamlit.app/)


## Main Functionalities

### Fare Prediction
The core functionality of our web application is the fare prediction. It is designed to estimate the cost of flights by prompting users to enter critical flight information. The details include:

- Origin airport
- Destination airport
- Departure date
- Departure time
- Cabin type

Once the ‘Predict’ button is clicked, the model processes these inputs to provide an estimated fare. For example, a user planning a trip from Atlanta Hartsfield-Jackson, GA (ATL) to Boston Logan International, MA (BOS) on a specific date and time, choosing coach class, will receive a predicted fare based on these inputs.

### Error Handling and User Experience
Our application is built with robust error handling to provide a seamless user experience. An example scenario includes:

- If a user selects the same airport for both origin and destination, an immediate flag is raised.
- The application displays a clear error message: “Origin and Destination airports cannot be the same. Please select different airports.”

This feature prevents user confusion and potential model errors, guiding them to provide valid inputs for accurate fare predictions. It is an integral part of our commitment to user-friendly design.

### Data-Driven Validations
We ensure a realistic and practical experience by validating the chosen route against actual flight data. For instance:

- If a user selects a route that is not serviced, such as from Newark (EWR) to John F. Kennedy (JFK) Airport, the app immediately identifies the issue.
- The user is alerted with the message: “There is no flight from EWR to JFK airport. Please select a different route.”

This validation process is essential for preventing fare predictions for non-existent flights, thereby maintaining the application’s reliability and accuracy. It also assists users in selecting viable flight options for their travel plans.

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

