# basic-ping-logger
Logs ping data to an excel file with a chart for plotting latency/packet drop issues.
![screenshot](image.png)

# Installation & Usage
> WARNING: Right now this script has a memory leak. You would have to run the script for a very long time to fill up your RAM, but ideally I need to store and update only deltas rather than the rewriting the entire excel file every time.

- `git clone https://github.com/crocokyle/basic-ping-logger.git`
- `cd basic-ping-logger`
- `pip install -r requirements.txt`
- `python main.py`

> NOTE: Excel files are created with the filename format timestamp `ping_data_{start_time}.xlsx` and stored in the `basic-ping-logger` directory.
