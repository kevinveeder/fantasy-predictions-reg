# NFL Fantasy Football Player Projections (2025)
This project uses real 2024 player statistics to train a simple linear regression model that predicts fantasy football performance for the upcoming 2025 season. It scrapes data from Pro Football Reference, FantasyPros projections, and ADP (Average Draft Position) rankings to generate full-season fantasy point predictions and highlight potential sleepers or overvalued players. This is done through custom web scraping functions that I had fun playing around with, hence why there is only one file in the repo. 

## Overview
- 2024 Player Data scraped and used to train a fantasy points per game (FPPG) prediction model
- Linear Regression Model trained using features like rush attempts, pass attempts, completions, and receptions
- 2025 Fantasy Projections scraped from FantasyPros for QBs, RBs, WRs, and TEs
- ADP Rankings merged in to compare model predictions against current draft expectations
- Final Output ranks the top 50 players based on predicted fantasy points and shows their current ADP

## Features Used for Modeling:
- `Att`: Rushing attempts per game
- `Tgt` Targets per game
- `Rec`: Receptions per game
- `Cmp`: Pass completions per game
- `Att.1`: Pass attempts per game

## Model Details
- Algorithm: Linear Regression (`sklearn`)
- Target Variable: Fantasy Points Per Game (`FFPG`)
- Training Data: 2024 season stats from Pro Football Reference
- Predictions: Applied to 2025 season projections (normalized per game and scaled back to full season)

---
