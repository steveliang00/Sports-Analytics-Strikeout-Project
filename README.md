# Strikeout Betting Project

**Have you ever wondered if it was possible to consistently profit from sports betting?**

For two months, I put my $200 on the line using a simple, easy-to-follow betting method to test this theory. This project analyzes the profitability of a sports betting strategy focused on MLB pitcher strikeouts, utilizing statistical techniques to identify positive expected value (+EV) bets.

## Project Overview
- **Goal**: To determine if using third-party projections (SaberSim) combined with Poisson distribution assumptions can consistently identify profitable betting opportunities against sportsbook lines.
- **Data**: Real betting data collected over a two-month period (June - August 2022).
- **Investment**: Initial bankroll of $200.

## Methodology
- **Projections**: Daily pitcher strikeout projections sourced from SaberSim.
- **Model**: Applied a Poisson distribution to the projections to calculate the probability of "Over" or "Under" outcomes for specific lines.
- **Betting Strategy**: Bets were placed only when the calculated "edge" (difference between modeled probability and implied odds) exceeded 5%.

## Key Findings
- **Overall Performance**: The experiment yielded a **Net Profit of $79.99** on the initial $200 investment (**~40% ROI**), with a total volume of **$8,618 wagered**.
- **Win Rate**: Achieved a **54.68%** win rate across 598 total bets.
- **Strategic Insights**:
    - The model demonstrated superior performance on specific Over/Under lines (specifically 2.5, 3.5, and 5.5).
    - Profitability showed variance across time periods, suggesting market efficiency shifts or model calibration factors.

## Conclusion
While the aggregate results showed volatility, the analysis **successfully identified a potentially profitable strategy**.

Through bootstrap analysis (10,000 simulations), a refined strategy focusing on the most effective O/U lines (2.5, 3.5, 5.5) during the optimal time period yielded a **statistically significant profit**, with a 95% confidence interval strictly above zero ($50.95 to $669.82). This indicates that with specific filtering and disciplined execution, the underlying method has valid predictive power and profit potential.

---
*Files:*
- `strikeout_betting_analysis.ipynb`: Complete analysis code, visualizations, and statistical testing.
- `strikeout_betting_analysis.html`: HTML export of the analysis with interactive graphs.
