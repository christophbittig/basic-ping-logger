# basic-ping-logger
Logs ping data to an excel file with a chart for plotting latency/packet drop issues.
![screenshot](image.png)

# Installation & Usage
> WARNING: Right now this script is essentially a memory leak. Don't run it for long periods of time. I need to only store and update deltas rather than the entire excel file

- `git clone https://github.com/crocokyle/basic-ping-logger.git`
- `cd basic-ping-logger`
- `pip install -r requirements.txt`
- `python main.py`

> Excel files are created with the filename format timestamp `ping_data_{start_time}.xlsx` in the `basic-ping-logger` directory.

