# Feature Selection BTC-Dataset
Feature selection in a dataset with bitcoin data.

The goal of making feature selection on a dataset before placing it in front of any machine learning process is to:
- `Reduce overfitting`: If we have more columns in the data than the number of rows, we will be able to fit our training data perfectly, but that **won’t generalize** to the new samples. And thus we learn absolutely nothing.
- `Occam’s Razor theorem`: We want our models to be **simple** and **explainable**. We lose explainability when we have a lot of features.
-  `Garbage In Garbage out`: Most of the times, we will have many non-informative features.  For Example, `Name` or `ID` variables Poor-quality input will produce Poor-Quality output.
    
In this jupyter notebook i will analyze a bitcoin dataset created by myself but which I will not make available. 

If you want you can build your own bitcoin dataset by looking at this repo: https://github.com/CristianCosci/bitcoin_OHLCV_dataset_generator and adding other data by referring to sites like https://www.blockchain.com/charts#currency and https://studio.glassnode.com/ through their API.

The dataset I will refer to will consist of the following features (Columns).

FEATURES :  [`'open', 'high', 'low', 'close', 'volume', 'new_addresses', 'active_addresses', 'total_unique_addresses', 'sending_addresses', 'receiving_addresses', 'total_fees', 'mean_transaction_fees', 'number_of_transaction', 'transaction_rate', 'market_cap', 'total_transaction_size', 'mean_transaction_size', 'hash_rate', 'mining_difficulty', 'reserve_risk', 'stock_to_flow', 'stock_to_fow_deflection', 'realized_profit', 'realized_loss', 'cvdd', 'address>001', 'addresses>1', 'exchanges_withdrawls', 'exchanges_deposits'`]

I will therefore select only the most useful features to predict the closing price of BITCOIN in USD.

The feature selection methodologies used are:
- **Boruta**
- **Pearson Correlation**
- **Regression Feature Selection**
- **Mutual Information Feature Selection**

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2FCristianCosci%2FBorutaPy_Feature_Selection_BTC_dataset&count_bg=%23880ED0&title_bg=%23555555&icon=proto-dot-io.svg&icon_color=%23E7E7E7&title=visite&edge_flat=false)](https://hits.seeyoufarm.com)
