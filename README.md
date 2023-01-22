# basic-ping-logger
Logs ping data to an excel file with a chart for plotting latency/packet drop issues.
![screenshot](image.png)

# Installation & Usage
> WARNING: Right now this script has a memory leak. You would have to run the script for a very long time to fill up your RAM, but ideally I need to store and update only deltas rather than the rewriting the entire excel file every time.

- `git clone https://github.com/crocokyle/basic-ping-logger.git`
- `cd basic-ping-logger`
- `pip install -r requirements.txt`
- `python pinger.py`

```
usage: pinger.py [-h] [-t TARGET] [-f SAVE_FREQUENCY] [-o OUTPUT_FILE]

optional arguments:
  -h, --help            show this help message and exit
  -t TARGET, --target TARGET
                        The host or IP address you want to test against. (default: 8.8.8.8)
  -f SAVE_FREQUENCY, --save-frequency SAVE_FREQUENCY
                        Number of pings to run between file saves. Should be a multiple of four. (default: 32)
  -o OUTPUT_FILE, --output-file OUTPUT_FILE
                        Output excel file. (default: ping_data_22-01-2023_16-28-48.xlsx)
```
