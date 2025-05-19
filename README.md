# TrendMiner Experimental SDK

The **TrendMiner Experimental SDK** is a Python client library for interacting with TrendMiner’s REST API. It provides object models, authentication helpers, and high-level data retrieval methods for time-series analytics.

## Installation

This SDK is in active development and not published on PyPI. Install the latest distribution directly from GitHub:

```bash
pip install https://github.com/TrendMinerCS/sdk/raw/main/sdk/trendminer_interface-0.1.dev900+ge76aa55-py3-none-any.whl
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
tags = tm.tag.by_name("TM-BP2*.1")
print(tags)
```
