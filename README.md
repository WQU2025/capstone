# Machine Learning for Algorithmic Trading Strategies
## Table of Contents
1. Loading and cleaning data, 
2. Feature engineering, 
3. HFT strategy
4. Backtesting

## Installation

pip install:
pandas numpy h5py matplotlib lightgbm scikit-learn

## Usage

1.	Prepare Data: Place H5 files for 002521 and 300132 in a folder (e.g., ./interview).
2.	Load and Clean Data: 
df_002521 = combine_h5_files('interview', '002521*.h5') 
df_002521 = clean_dataframe(df_002521) 
df_002521 = sort_by_datatime(df_002521) 
df_002521 = reduce_column_size(df_002521)

3.	Engineer Features:
df_002521_signals = generate_level2_imbalance(df_002521) 
df_002521_signals = add_rolling_volatility(df_002521_signals, window='5min')
4.	Implemetation: Resample, generate signals, and backtest 
       

## Contributions are welcome! Please open issues or submit pull requests.

