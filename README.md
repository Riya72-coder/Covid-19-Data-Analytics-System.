# COVID-19 Data Analytics System 

## Overview
This project is a COVID-19 Data analytics system that provides insights into the pandemic using data visualizations, sentiment analysis, and predictive modeling. It allows users to analyze trends, visualize correlations, and predict COVID-19 cases based on input data. Built using Python and Flask, this project showcases interactive graphs and tables to deliver meaningful information about the pandemic.

## Features
- **Interactive Dashboard**: Displays line plots, bar charts, heatmaps, and pie charts for COVID-19 data.
- **Sentiment Analysis**: Analyzes public sentiment data by state and visualizes weighted sentiments.
- **Predictive Modeling**: Uses machine learning to predict COVID-19 case trends.
- **Dynamic Tables**: View detailed state-wise sentiment data on a separate page.
- **User-Friendly Design**: Clean and responsive interface with Bootstrap integration.

## 📊 Visualizations

### Line Plot - Trends Over Time
![Trends Over Time](static/images/trends_over_time.png)

### Forecast Covid-19
![Forecast Covid-19](static/images/arima_forecast.png)

### Heatmap correlation
![Heatmap correlation](static/images/correlation_heatmap.png)

### Sentiment Distribution
![Sentiment Distribution](static/images/sentiment_distribution.png)

### Top 10 States Cases
![Top 10 States Cases](static/images/top_10_states_cases.png)

## Installation
### Prerequisites
- Python 3.8 or higher
- Pip (Python package manager)
- A code editor (e.g., PyCharm)

### Steps
1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/Riya72-coder/Covid-19-Data-Analytics-System..git
   ```

2. Navigate to the project directory:
   ```bash
   cd covid-dashboard
   ```

3. Install the required Python libraries:
   ```bash
   pip install -r requirements.txt
   ```

4. **Dataset & Optimization**
   This project utilizes COVID-19 datasets sourced from Kaggle, covering sentiments, vaccination rates, and daily case statuses.

   Note on Performance: To ensure high-speed loading and compatibility with serverless deployment (Vercel), the raw datasets have been pre-processed and optimized. Unused features were pruned to reduce the application footprint while maintaining full analytical integrity.

   **Main Dataset:** data/output.csv (Optimized)

   **Sentiment Data:** data/COVID-19_Sentiments.csv (Optimized)

   **Vaccination Data:** data/IndiaCovidVaccination2023.csv (Optimized)

   All necessary data is included in the repository; no external downloads are required to run the dashboard locally.

   **Action:** Place these CSV files inside the `data/` folder of this project.

5. Run the Flask application:
   ```bash
   python flask_app.py
   ```

6. Open your browser and navigate to:
   ```plaintext
   http://127.0.0.1:5000/
   ```

## Project Structure
```plaintext
covid-19-project/
├── data/                      # Folder for CSV datasets
├── static/                    # CSS and image assets (plots and graphs)
├── templates/                 # HTML templates (dashboard.html)
├── build_data.py              # Main data analysis and visualization script
├── flask_app.py               # Main Flask application
├── covid_model.pkl            # Pre-trained machine learning model
└── requirements.txt           # Python dependencies
```

## Technologies Used
- **Backend**: Flask (Python)
- **Frontend**: HTML, CSS, Bootstrap
- **Data Visualization**: Matplotlib, Seaborn
- **Machine Learning**: Scikit-learn
- **Data Processing**: Pandas, NumPy

## How to Use the Project
1. **View the Dashboard**: Open the main dashboard page to see COVID-19 visualizations and insights.
2. **Access Sentiment Data**: Click on the "View Weighted Sentiment by State" link to explore detailed sentiment data.
3. **Predict Cases**: Enter a numerical input on the prediction page to see the model's forecast of COVID-19 cases.

## License
This project is licensed under the [MIT License](LICENSE). You are free to use, modify, and distribute this project with 
proper attribution.

## Acknowledgments
- Thanks to [John Hopkins University](https://github.com/CSSEGISandData/COVID-19) for providing the COVID-19 dataset.
- Special thanks to the team members and contributors who supported this project.
- Libraries and frameworks: Flask, Matplotlib, Bootstrap, Scikit-learn.

---
Feel free to contribute to this project by submitting issues or pull requests!
