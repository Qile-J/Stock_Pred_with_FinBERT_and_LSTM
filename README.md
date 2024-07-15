# AAPL Stock Prediction Pipeline

## Project Overview
This project demonstrates a pipeline for stock prediction using Apple Inc. (AAPL) as an example. The pipeline includes web scraping, data collection, and model training, combining FinBERT-based sentiment analysis with BiLSTM time-series forecasting.

## Data
`AAPL_Merge_2024-07-10.csv`: A CSV file with historical stock price data, sentiment scores, and the number of news headlines analyzed for each day.

## Source Code
- `BiLSTM.ipynb`: A Jupyter notebook for training the BiLSTM model using the merged data.
- `update_data.ipynb`: A Jupyter notebook to collect the most recent stock price data.
- `update_news.ipynb`: A Jupyter notebook to scrape the web for news articles related to AAPL, save the news headline summary and other information, and perform sentiment analysis with FinBERT to extract an average sentiment score for each day.

## Instructions
1. **Update Data**: Run `update_data.ipynb` to fetch the latest stock price data. 
2. **Update News**: Run `update_news.ipynb` to scrape news articles, perform sentiment analysis using FinBERT, and update the data file. Ensure you update the `your_api_key` and data directory accordingly.
3. **Train Model**: Use `BiLSTM.ipynb` to train the BiLSTM model on the combined dataset.

## References
- [FinBERT: A Pretrained Language Model for Financial Communications](https://arxiv.org/abs/1908.10063)
- [BiLSTM Model](https://github.com/TheQuantScientist/FeatureEngineering-BiLSTM)

## Notes
- Ensure you have the necessary dependencies installed, such as `numpy`, `pandas`, `matplotlib`, `requests`, and `transformers`.
