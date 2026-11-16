# Bitcoin Price Prediction from Chainlets, Explained with SHAP

Predicts the daily Bitcoin price for every day of December 2017 (one-day-ahead horizon) from lagged prices and Bitcoin transaction-graph chainlet features, using both the occurrence and the amount chainlet files. The model is explained with SHAP.

UCF, Master's in Financial Technology, CAP 5619 homework.

## Data

The three course files (`OccChainletsInTime.txt`, `AmoChainletsInTime.txt`, `pricedBitcoin2009-2018.csv`) are not redistributed. The notebook downloads them into `data/` on the first run from the course repository, https://github.com/cakcora/BitcoinChainnet.

## Run

1. Use Python 3.9 or newer, ideally in a virtual environment.
2. `pip install -r requirements.txt`. The first notebook cell also installs anything that is missing.
3. Open `btc_chainlet_xai.ipynb` and run all cells.

## Output

Running the notebook writes `december_2017_predictions.csv`: the predicted price for each day of December 2017, in dollars, with the columns `date` and `predicted_price`. A copy from the last run is tracked in this repository.
