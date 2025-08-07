
# EV Adoption Forecasting

This project is an interactive web dashboard built using Streamlit to forecast Electric Vehicle (EV) adoption trends in various counties of Washington State. The model predicts the number of EVs over the next 3 years based on historical data and engineered features.

## ðŸ“Œ Features

- Interactive county selection
- Time series forecasting using a machine learning model
- Visualization of historical and forecasted EV adoption trends
- Multi-county comparison of forecasted growth
- Cumulative EV adoption graph with clear markers

## ðŸ§  Modules Used

- `streamlit`
- `pandas`
- `numpy`
- `matplotlib`
- `joblib`
- `datetime`

## ðŸ›  How it Works

1. Loads preprocessed EV data (`preprocessed_ev_data.csv`) and a pre-trained forecasting model (`forecasting_ev_model.pkl`).
2. User selects a county to forecast EV adoption.
3. The model generates a 36-month forecast using lag features and rolling statistics.
4. Data is visualized using matplotlib inside Streamlit.
5. Optionally, users can compare forecasts across up to 3 counties.

## ðŸ§¾ Data

The dataset contains monthly EV adoption data per county in Washington, with additional features like lag values, rolling means, and percentage changes used for forecasting.

## ðŸš€ Getting Started

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/ev-forecast-dashboard.git
    cd ev-forecast-dashboard
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the app:
    ```bash
    streamlit run app.py
    ```

Make sure the following files are present in the root directory:
- `forecasting_ev_model.pkl`
- `preprocessed_ev_data.csv`
- `ev_wallpage.jpg`

## ðŸ™ Acknowledgements

- Developed as part of the **AICTE Internship Cycle 2**.
- Guidance and mentorship support provided by **AICTE mentors and coordinators**.
- Project inspiration based on real-world EV adoption trends and the importance of sustainable transportation planning.

---

Prepared by **Dharma Satya Teja Kolla**
