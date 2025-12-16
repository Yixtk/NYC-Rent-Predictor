# NYC Rent Predictor

A web-based Monte Carlo simulation tool for predicting NYC rental prices based on borough, property type, and move-in month.

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

Base rents and seasonal factors are derived from median asking rent data analysis.

