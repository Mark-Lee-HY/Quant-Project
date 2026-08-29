Introduction:

This project presents a quantitative trading strategy implemented for cryptocurrency markets: Cross-sectional Risk-Adjusted Momentum Strategy. This strategy leverages historical price data to generate dynamic trading signals that aim to outperform passive benchmarks like buy-and-hold strategies.

Data Collection and Preprocessing:

The data was sourced from Binance via its API and includes multiple major cryptocurrencies such as BTC, ETH, ADA, BNB, DOT, XRP, etc. The data covered the period from January 2020 to December 2025 and was sampled at a 1-hour frequency. The January 2020 - December 2023 period was used as the training set, and January 2024 - December 2025 was used as the validation set. For each asset, price data were collected, followed by the computation of logarithmic returns and signal construction.

Optimisation:

A grid search was conducted over various variables such as LOOKBACK_HOURS (e.g., 168, 336, 720, 2160) and SKIP_HOURS (e.g., 0, 6, 12, 24) to identify the optimal parameters for the lookback signal. The resulting Sharpe ratios for each combination were plotted on a heatmap to visualise the most effective configurations. The final portfolio signal were created by the heatmap estimates. Figure 1 is a demonstration of an optimisation heatmap for the Cross-sectional Risk-adjusted Momentum Strategy as an example.

