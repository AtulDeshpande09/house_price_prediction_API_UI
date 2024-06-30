# Predicting House Prices with Machine Learning: A REST API and User Interface

## Project Description
This project involves developing a machine learning model to predict house prices based on various features. The solution includes a Flask-based REST API for making predictions and a user-friendly interface created using Tkinter to interact with the model.

## Features
- **Machine Learning Model**: Predicts house prices based on input features.
- **Flask API**: Provides an endpoint to get predictions from the model.
- **User Interface**: Simple Tkinter-based GUI to interact with the prediction API.

## Technologies Used
- **Programming Language**: Python
- **Libraries**: Flask, pandas, joblib, requests, Tkinter
- **Machine Learning**: Scikit-learn

## Installation and Setup

### Prerequisites
- Python 3.x
- Required Python packages (see `requirements.txt`)

### Steps
1. **Clone the repository**:
    ```bash
    (https://github.com/AtulDeshpande09/house_price_prediction_API_UI.git)
    cd house_price_prediction_API_UI
    ```

2. **Install dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

3. **Run the Flask API**:
    ```bash
    python house_price_api.py
    ```

4. **Run the User Interface**:
    ```bash
    python house_price_test.py
    ```

5. **Run for Graphical User Interface**:
    ```bash
    python ui.py
    ```

## Usage

### API Endpoint
- **URL**: `/predict`
- **Method**: POST
- **Payload**: JSON object with the following fields:
    ```json
    {
        "bedrooms": int,
        "bathrooms": int,
        "sqft_living": int,
        "age_of_house": int
    }
    ```
- **Response**: JSON object with the predicted price:
    ```json
    {
        "prediction": float
    }
    ```

### User Interface
1. Launch the Tkinter interface by running `python ui.py`.
2. Enter the required house details (bedrooms, bathrooms, sqft living area, age of the house).
3. Click on "Get Prediction" to see the predicted house price.

## Contributing
Contributions are welcome.

## License
This project is licensed under the Apache-2.0 License.

## Acknowledgments
- Special thanks to the open-source community for the tools and libraries used in this project.
