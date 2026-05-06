# Moving Average Strategy
The notebook currently uses Apple (`AAPL`) as the default ticker, downloads historical prices with `yfinance`, calculates moving averages, simulates basic buy and sell decisions, and plots the strategy performance.

## What the Strategy Does

The strategy compares a short moving average with a long moving average:

- Short moving average: 20 days
- Long moving average: 50 days
- Buy signal: the short moving average crosses above the long moving average
- Sell signal: the short moving average crosses below the long moving average

The notebook supports both:

- Simple moving average, selected with `"s"`
- Exponential moving average, selected with `"e"`

## Requirements

This project uses Python and Jupyter Notebook. The main Python packages are:

- `yfinance`
- `pandas`
- `matplotlib`
- `jupyter`

Install them with:

```bash
pip install yfinance pandas matplotlib jupyter
```

## How to Run

1. Open the project folder.
2. Start Jupyter Notebook:

```bash
jupyter notebook
```

3. Open `MA_strategy.ipynb`.
4. Run the notebook cells from top to bottom.

You can change the stock ticker near the top of the notebook:

```python
TICKER = "AAPL"
```

You can also change the starting cash:

```python
cash = 5000
```


## READ THIS !!

This project is for learning and experimentation only. It is not financial advice, and the strategy does not account for taxes, trading fees, slippage, or risk management.
