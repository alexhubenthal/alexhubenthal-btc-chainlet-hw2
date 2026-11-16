# Predicting December 2017 Bitcoin Prices from Chainlets

A ridge regression predicts the Bitcoin price one day ahead for each day in December 2017, from past prices and the daily chainlet counts and amounts. Both course chainlet files are used. SHAP shows what pushed each prediction up or down.

Homework for CAP 5619, AI for Finance, in the UCF Master's in Financial Technology program.

## Data

The three course files (`OccChainletsInTime.txt`, `AmoChainletsInTime.txt`, `pricedBitcoin2009-2018.csv`) are not redistributed. The notebook downloads them into `data/` on the first run from the course repository, https://github.com/cakcora/BitcoinChainnet.

## Run

1. Use Python 3.9 or newer, ideally in a virtual environment.
2. `pip install -r requirements.txt`. The first notebook cell also installs anything that is missing.
3. Open `btc_chainlet_xai.ipynb` and run all cells.

The notebook gives the same predictions on Python 3.9 with pandas 2.2 and on Python 3.13 with pandas 3.1.

## Output

Running the notebook writes `december_2017_predictions.csv`: the predicted price for each day of December 2017, in dollars, with the columns `date` and `predicted_price`. A copy from the last run is tracked in this repository.
