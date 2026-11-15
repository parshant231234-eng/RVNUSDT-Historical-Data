# RVNUSDT 1-Minute Historical Kline Dataset

An institutional-grade, open-source archive of cleaned, standardized, and validated **1-minute intraday historical kline data** for **RVNUSDT** (Binance Spot).

---

## 📊 Dataset Specifications
- **Symbol:** `RVNUSDT`
- **Market:** Binance Spot
- **Timeframe:** 1 Minute (`1m`)
- **Total Months:** `87` months
- **Total Candles:** `3,752,211` 1-minute candles
- **Historical Range:** `2019-09-25 12:00:00` to `2026-11-14 23:59:00` (UTC)
- **Schema:** `timestamp, datetime_utc, open, high, low, close, volume, quote_volume, trade_count, taker_buy_volume, taker_buy_quote_volume`

---

## 🏛️ Directory Hierarchy
```text
RVNUSDT-Historical-Data/
├── README.md
└── 1m/
    └── <YYYY>/
        └── <MM>/
            └── RVNUSDT_1m_<YYYY-MM>.csv
```

---

## ⚡ 1-Line Pandas Stream Loader
Load any month directly from GitHub's raw CDN without cloning the repository:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/parshant231234-eng/RVNUSDT-Historical-Data/main/1m/2026/11/RVNUSDT_1m_2026-11.csv"
df = pd.read_csv(url)
print(df.head())
```
