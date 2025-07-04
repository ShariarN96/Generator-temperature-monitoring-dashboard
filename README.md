# 🔥 Generator Temperature Monitoring Dashboard

An interactive dashboard built in **Python** using **Dash** and **Plotly** to monitor and forecast generator temperatures. This tool provides an intuitive interface for engineers and analysts to explore temperature trends, adjust model parameters, and predict potential overheating or failure scenarios.

---

## 🧠 Methodology

To enable predictive insights, we first identified the most influential variables affecting generator temperature. Based on correlation analysis and domain understanding, we selected **ambient temperature** and **electrical current** as the two key input features.

The dashboard was then designed with:

- Custom controls to adjust these parameters
- A date range picker for filtered time-series analysis
- Real-time visual feedback through interactive plots

This structure allows users to simulate and explore temperature behavior under varying operational conditions.

---

## 📊 Dashboard Demo

Below is a short demo of the dashboard in action:  
👉 *[https://shanenn.carrd.co/assets/videos/video01.mp4?v=db187847]*

Users can:
- Adjust model parameters dynamically
- Visualize historical and predicted temperatures
- Select custom timeframes for focused analysis

---

## 💻 Python Code

The full source code is available on GitHub:  
🔗 [View the Code on GitHub](https://github.com/ShariarN96/Generator-temperature-monitoring-dashboard)

Here's a snippet showing part of the core Python logic:

> *(Insert a code snippet image or use Markdown code blocks if preferred)*

```python
# Sample code preview
import pandas as pd
from sklearn.linear_model import LinearRegression

# Load and prepare data
df = pd.read_csv("generator_data.csv")
X = df[["ambient_temp", "current"]]
y = df["generator_temp"]

# Train model
model = LinearRegression()
model.fit(X, y)
