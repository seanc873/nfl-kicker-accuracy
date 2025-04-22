# NFL Kicker Accuracy
This project analyzes NFL field goal and extra point kicks with the goal of evaluating kicker performance through **context-aware statistical modeling**. Using play-by-play tracking data, game conditions, and weather variables, we estimate expected field goal success (xFG) and identify factors influencing kicker accuracy.

## 📊 Objective

To construct robust models that:
- Estimate the probability a kick is made, adjusting for context (e.g., weather, field location, game state)
- Quantify kicker performance using **Rao-Blackwellized estimates**
- Provide fair comparisons across kickers and teams by adjusting for kick difficulty

## 🧠 Methods

- **Data Sources**: NFL tracking data and play-by-play logs ([**BDB 2022**](https://www.kaggle.com/competitions/nfl-big-data-bowl-2022/data)), and historical weather data ([**ThompsonJamesBliss**](https://github.com/ThompsonJamesBliss/WeatherData))
- **Feature Engineering**:
  - Kick location and angle
  - Weather: wind speed/direction, temperature, humidity, precipitation
  - Game state: score differential, quarter, time remaining
- **Modeling Approaches**:
  - Logistic and multivariable regression
  - Rao-Blackwellization for variance reduction
  - Exploratory visualizations (scatterplots, heatmaps)