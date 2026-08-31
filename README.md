# CBU-NPL-Monte-Carlo-Simulation
Monte Carlo simulation of Uzbekistan's banking-sector NPL risk, capital stress, built on real Central Bank of Uzbekistan (CBU) disclosures (June 2026). Models a one-factor systemic shock across state-owned vs. private/foreign banks, runs 20,000 iterations in Python, and visualizes risk distributions in Power BI.

# CBU Fintech Risk Monitoring — Monte Carlo NPL & Capital Stress Simulation

Independent project simulating Uzbekistan's banking-sector non-performing
loan (NPL) risk and capital-buffer erosion using a Monte Carlo, one-factor
stress model — the same analytical approach used in supervisory stress
testing. Built on real, published Central Bank of Uzbekistan (CBU) data
(loan portfolio size, NPL ratios, capital adequacy ratio, provisioning
coverage as of June 2026).

## What it does
- Splits the loan portfolio into state-owned vs. private/foreign bank
  segments (different risk profiles)
- Applies a one-factor shock model: a shared systemic factor plus
  segment-specific idiosyncratic noise
- Runs 20,000 Monte Carlo iterations in Python (NumPy/Pandas)
- Outputs a full probability distribution of NPL outcomes and capital
  erosion, visualized in Power BI

## Key result
Simulated mean NPL ratio of 3.73% closely matches the actual reported
figure of 3.7% (June 2026), validating model calibration. 95th-percentile
capital erosion from uncovered NPLs is ~1.56% of total banking capital.

## Tools
Python (NumPy, Pandas, Matplotlib) · Jupyter Notebook · Power BI

## Data sources
Central Bank of Uzbekistan (cbu.uz) Financial Stability Report 2025;
CBU data as reported by UzDaily.uz and Xinhua, June 2026; INVEXI summary
of CBU 2025 outcomes.

## Files
- monte_carlo_npl_risk.ipynb — simulation notebook
- npl_monte_carlo_simulations.csv — full 20,000-row simulation output
- npl_monte_carlo_summary.csv — summary percentiles
- dashboard.pdf / dashboard.png — Power BI dashboard export


