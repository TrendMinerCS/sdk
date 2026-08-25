# TrendMiner Python SDK

Python client library for the TrendMiner REST API — object models, authentication
helpers, and high-level data retrieval for time-series analytics.

## Pick your TrendMiner release

The SDK is versioned against TrendMiner releases. **Use the docs that match your
appliance**, not the newest ones — the API surface differs between releases.

| TrendMiner release | Documentation | Wheel |
| --- | --- | --- |
| preview | [Read the docs](preview/authentication.md) | [Download](https://github.com/TrendMinerCS/sdk/tree/main/sdk) |

Not sure which release you are on? Once you have a client:

```python
print(client.appliance.get_version())
```

## Using these docs with an AI assistant

Every release ships a single plain-text bundle built for chatbot ingestion — the
full API surface, worked examples, and explicit constraints in one file.

**For preview:**

```
https://trendminercs.github.io/sdk/preview/llms-full.txt
```

Point your assistant at that URL, or download it and attach it to the
conversation. Attaching is more reliable — many enterprise assistants have URL
fetching disabled.

Then ask for what you want, for example:

> Using the attached TrendMiner SDK documentation, write a script that
> authenticates against our appliance and lists all tags matching "TI-*".

A short index for tools that look for it lives at
[`llms.txt`](https://trendminercs.github.io/sdk/preview/llms.txt).

!!! warning "Match the bundle to your appliance"
    The bundle states the release it documents in its header. Giving an assistant
    the wrong release is the most common cause of generated code that looks
    correct but fails at runtime.

## Installation

The SDK is not on PyPI. Install the wheel for your release directly from this
repository — see the [README](https://github.com/TrendMinerCS/sdk#readme) for the
exact command.
