# DCF-analysis-using-Monte-Carlo-Sim
This project implements a Monte Carlo simulation-based approach to estimate the intrinsic value of a company using the Discounted Cash Flow (DCF) model. Instead of relying on single-point estimates, it incorporates uncertainty in key assumptions by assigning probability distributions and running multiple simulation trials to generate a more robust valuation range.
Methodology
Forecast Free Cash Flow to Firm (FCFF):
Projected future FCFF based on expected EBIT, tax rate, reinvestment rate, and terminal growth assumptions.

Randomization via Monte Carlo:
Key input variables (e.g. EBIT, reinvestment rate, WACC, terminal growth) are assigned probability distributions and simulated using Python's random library to reflect realistic variation.

DCF Valuation across Simulations:
For each simulation, DCF is computed using:

Mid-year convention for discounting

Terminal value using Gordon Growth Model

Aggregation of discounted cash flows

Results Visualization:
A histogram of simulated firm values provides an intuitive view of the valuation range, including key percentiles like 10th, 50th (median), and 90th.

Libraries Used
numpy – numerical calculations

pandas – data manipulation

matplotlib.pyplot – visualization

random – sampling from probability distributions

Output
The simulation produces a distribution of firm values, offering insight into the range and likelihood of potential valuations rather than a single deterministic value. This approach helps in risk-aware investment decision making.
