# NYC Rent Predictor

A web-based Monte Carlo simulation tool for predicting NYC rental prices based on borough, property type, and move-in month.

🌐 **Live Demo:** [https://yixtk.github.io/NYC-Rent-Predictor/](https://yixtk.github.io/NYC-Rent-Predictor/)

## Features

- Three-layer Monte Carlo model for rent prediction
- Borough-specific predictions (Manhattan, Brooklyn, Queens, Bronx, Staten Island)
- Property types: Studio, 1BR, 2BR, 3BR
- Seasonal factors based on median asking rent data
- 3% annual inflation rate
- 10,000 simulation runs for accurate probability distributions

## Usage

Simply open `predictor.html` in any modern web browser. No installation or server required.

## Model Description

**Layer 1 (Deterministic):** Base rent × Annual trend (3% inflation) × Seasonal factor

**Layer 2 (Stochastic):** Market noise (±5%) + Borough variation (±8-18%)

**Layer 3 (Aggregation):** 10,000 simulations → Probability distribution

## Data Sources

- **Base Rents:** Derived from NYC median asking rent data (2024), scaled by borough and property type
- **Seasonal Factors:** Calculated from historical median asking rent patterns (2010-2025)
- **Annual Inflation:** Set at 3% per year based on recent rental market trends
- **Source:** NYC Median Asking Rent dataset

## Tech Stack

- Pure HTML/CSS/JavaScript
- React 18 (via CDN)
- Tailwind CSS
- No build process required - runs directly in browser

## Contributing

Feel free to open issues or submit pull requests for improvements!

