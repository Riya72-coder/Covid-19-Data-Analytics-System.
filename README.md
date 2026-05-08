# 🦠 COVID-19 India Data Analytics System

A premium, high-performance data analytics dashboard providing real-time insights into the COVID-19 pandemic in India through interactive visualizations, AI forecasting, and public sentiment analysis.

![Dashboard Preview](static/images/trends_over_time.png)

## ✨ Key Features

- **💎 Premium UI/UX**: A state-of-the-art dark mode interface featuring glassmorphism, fluid animations (AOS), and a modern aesthetic designed for clarity and impact.
- **📈 Real-Time Interactive Charts**: Powered by Chart.js 4.4.3, featuring dynamic trends, state-wise distributions, and proportional case analysis.
- **🤖 AI Forecasting**: Integrated ARIMA and Facebook Prophet models to predict case trajectories for the next 30 days.
- **🧠 Sentiment Analysis**: Advanced visualization of public sentiment data across different Indian states, derived from social media data.
- **⚡ Performance Optimized**: 
  - **Zero Junk**: Resolved 17s `requestAnimationFrame` violations using intelligent task scheduling.
  - **Idle Rendering**: Uses `requestIdleCallback` to animate KPI counters without blocking the main thread.
  - **Fast Load**: Pre-processed 19MB JSON data bridge for near-instant chart rendering.
- **🛡️ Secure Assets**: Fixed cross-origin tracking prevention issues and CORS storage violations for CDN-hosted libraries.

## 📊 Visualizations Included

### 📉 Trends Over Time
Dynamic line charts showing the daily progression of Total Cases, Recoveries, and Deaths.
![Trends Over Time](static/images/trends_over_time.png)

### 🔮 AI Predictions
Time-series forecasting using statistical models (ARIMA) and additive models (Prophet).
![Forecast](static/images/arima_forecast.png)

### 🗺️ State Analysis
Horizontal bar charts of Top 10 States and Proportional Pie charts for the Top 5 most impacted regions.
![Top 10 States](static/images/top_10_states_cases.png)

### 💬 Sentiment & Correlation
Doughnut charts for sentiment distribution and heatmaps showing correlations between vaccination rates and case counts.
![Heatmap](static/images/correlation_heatmap.png)

## 🚀 Getting Started

### Prerequisites
- **Python 3.8+**
- **pip** (Python Package Manager)

### Installation
1. **Clone the repository:**
   ```bash
   git clone https://github.com/Riya72-coder/Covid-19-Data-Analytics-System..git
   cd covid-19-project
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Data Setup:**
   Ensure the following CSV files are present in the `data/` directory:
   - `output.csv` (Main Dataset)
   - `COVID-19_Sentiments.csv` (Sentiment Data)
   - `IndiaCovidVaccination2023.csv` (Vaccination Data)

4. **Run the Server:**
   ```bash
   python flask_app.py
   ```

5. **Access the Dashboard:**
   Open [http://127.0.0.1:5000/dashboard](http://127.0.0.1:5000/dashboard) in your browser.

## 🛠️ Technology Stack

- **Backend**: Flask (Python)
- **Frontend**: HTML5 (Semantic), Vanilla CSS (Custom Design System), Bootstrap 5.3
- **Charts**: Chart.js 4.4.3 (Custom Dark Theme)
- **Animations**: AOS (Animate On Scroll)
- **Data Science**: 
  - **Processing**: Pandas, NumPy
  - **Visualization**: Matplotlib, Seaborn
  - **Forecasting**: Statsmodels (ARIMA), Scikit-learn
- **Data Injection**: Jinja2 with JSON Bridge pattern

## 📂 Project Structure
```plaintext
covid-19-project/
├── data/                  # Raw and processed CSV datasets
├── static/
│   ├── css/               # Modern Design System (style.css)
│   └── images/            # Generated analytical plots
├── templates/
│   ├── dashboard.html     # Main analytics interface
│   └── covid-info.html    # Educational information center
├── build_data.py          # Data processing & visualization engine
├── flask_app.py           # Web server & API routing
├── requirements.txt       # Project dependencies
└── dashboard_data.json    # Pre-computed analytics bridge
```

## 📝 License
This project is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments
- **Ministry of Health & Family Welfare (MoHFW)** for official Indian COVID-19 data.
- **John Hopkins University** for global dataset standards.
- **Kaggle** for the diverse sentiment and vaccination datasets.

---
⭐ If you find this project useful, give it a star on GitHub!
