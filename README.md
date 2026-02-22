📊 Trader Sentiment Analysis

Quantitative Analysis of Fear vs Greed Impact on Trader Behavior

📌 Project Overview

This project analyzes how market sentiment regimes (Fear vs Greed) influence trader performance and behavior. By combining historical trading data with a daily sentiment classification dataset, the project investigates whether traders behave differently under varying emotional market conditions and whether performance metrics such as PnL, win rate, and drawdown differ across regimes.

The analysis is structured to move from raw trade-level data to daily aggregated trader metrics, followed by sentiment-based comparisons, segmentation analysis, and finally actionable trading rules.

🎯 Objectives

1. The primary objectives of this project are:

2. To determine whether performance (PnL, win rate, drawdown proxy) differs between Fear and Greed days

3. To analyze whether traders change behavior based on sentiment (trade frequency, exposure, directional bias)

4. To segment traders into meaningful groups (high/low exposure, frequent/infrequent, consistent/inconsistent)

5. To derive sentiment-adaptive trading rules

📂 Datasets Used

This project uses two datasets:

1. Historical Trader Dataset

2. Fear & Greed Dataset



🏗️ Project Workflow

The analysis follows a structured quantitative pipeline:

1. Data loading and inspection

2. Data cleaning and timestamp conversion

3. Daily-level aggregation of trader metrics

4. Sentiment alignment by date

5. Performance comparison across Fear vs Greed regimes

6. Behavioral analysis (frequency, exposure, long/short ratio)

7. Trader segmentation

8. Strategy formulation

📊 Key Metrics Created:

* The following derived metrics are used in the analysis:

* Daily PnL per trader

* Trade count per day

* Win rate

* Average trade size

* Exposure proxy (Size USD)

* Drawdown proxy using cumulative PnL

📈 Key Insights

Some of the major findings from the analysis include:

* Fear days exhibit higher volatility and weaker average PnL

* Traders tend to increase activity during extreme sentiment regimes

* Exposure spikes during Fear periods correlate with larger drawdowns

* Consistent traders perform relatively better during Greed periods

* Behavioral changes are observable across sentiment regimes

🚀 Strategy Recommendations

Based on the findings, two regime-adaptive rules were proposed:

* During Fear days, reduce exposure for high-exposure and frequent traders to limit drawdowns

* During Greed days, selectively increase exposure for consistent traders

These rules demonstrate how sentiment signals can be converted into structured risk management adjustments.

🛠️ Technology Stack

This project was developed using:

* Python 3

* Pandas

* NumPy

* Matplotlib

*Seaborn

* Google Colab

⚙️ Setup Instructions:

Option 1: Run in Google Colab (Recommended)

1. Open Google Colab

2. Upload Trader_Sentiment_Analysis.ipynb

3. Upload both datasets

4. Run all cells sequentially


Option 2: Run Locally

Step 1: Clone the repository

```
git clone https://github.com/your-username/trader-sentiment-analysis.git
cd trader-sentiment-analysis
```

Step 2: Create a virtual environment (recommended)

```
python -m venv venv
```
Activate environment:

Windows:
```
venv\Scripts\activate
```
Mac/Linux:
```
source venv/bin/activate
```
Step 3: Install required packages
```
pip install pandas numpy matplotlib seaborn jupyter
```
Step 4: Run Jupyter Notebook

jupyter notebook

Open:
```
Trader_Sentiment_Analysis.ipynb
```
Run all cells from top to bottom.


To reproduce results:

Ensure both datasets are in the same directory as the notebook

Execute all notebook cells sequentially

Do not skip preprocessing steps

The analysis is deterministic and fully reproducible.
