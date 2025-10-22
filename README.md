# TrendMiner Experimental SDK

The **TrendMiner Experimental SDK** is a Python client library for interacting with TrendMiner’s REST API. It provides object models, authentication helpers, and high-level data retrieval methods for time-series analytics.

## Installation

This SDK is in active development and not published on PyPI. Install the latest distribution directly from GitHub based on your current TrendMiner version:

### 2025R3
```bash
pip install https://github.com/TrendMinerCS/sdk/raw/main/sdk/2025R3/trendminer_interface-0.1.0.post205-py3-none-any.whl
```

### 2025R2
```bash
pip install https://github.com/TrendMinerCS/sdk/raw/main/sdk/2025R2/trendminer_interface-0.0.0-py3-none-any.whl
```

### 2025R1
```bash
pip install https://github.com/TrendMinerCS/sdk/raw/main/sdk/2025R1/trendminer_interface-0.1.0.post161+86ad9f74.dirty-py3-none-any.whl
```

### 2024R3.1
```bash
pip install https://github.com/TrendMinerCS/sdk/raw/main/sdk/2024R3.1/trendminer_interface-0.1.0.post160+1848287a.dirty-py3-none-any.whl
```

### 2024R2.1
```bash
pip install https://github.com/TrendMinerCS/sdk/raw/main/sdk/2024R2.1/trendminer_interface-0.1.0.post162+bc00a459.dirty-py3-none-any.whl
```

## Quick Start

```python
from trendminer_interface import TrendMinerClient

# Initialize client with API credentials
tm = TrendMinerClient(
    url="https://your-trendminer-instance.com",
    client_id="YOUR_CLIENT_ID",
    client_secret="YOUR_CLIENT_SECRET",
    tz="Europe/Brussels"
)

# Example: search for tags by name
tags = tm.tag.search(name="TM-BP2*.1")
print(tags)
```
