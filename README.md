# 🛒 E-Commerce Demand Forecasting

End-to-end demand forecasting pipeline on UCI Online Retail dataset (541K transactions).

## 📊 Project Overview
- **Dataset**: UCI Online Retail (Dec 2010 – Dec 2011)
- **Records**: 541,909 transactions
- **Tools**: PySpark · HDFS · Python · Power BI

## ⚙️ Data Engineering
- Cleaned 541K transactions using PySpark
- Flagged cancelled orders & extracted temporal features
- Stored on HDFS partitioned by YearMonth (replication factor 3)
- Achieved **3.89x speedup** using caching & optimized partitioning

## 📈 Data Analysis (EDA)
- Monthly Revenue Trend — Q4 seasonal spike detected
- RFM Analysis → 5 customer segments
- Retention Analysis → **65.59%** retention rate
- Cancellation Analysis → **£896K** lost revenue
- Product Portfolio Matrix → 3,922 products classified

## 🔑 Key Results
| Metric | Value |
|--------|-------|
| Total Revenue | £10.6M |
| Unique Customers | 4,339 |
| Retention Rate | 65.59% |
| Cancellation Rate | 1.72% |
| Lost Revenue | £896K |

## 🛠️ Tech Stack
- PySpark
- HDFS
- Python (Matplotlib, Seaborn)
- Power BI & DAX
