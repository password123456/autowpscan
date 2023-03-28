# autowpscan
![made-with-python][made-with-python]
![Python Versions][pyversion-button]
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fpassword123456%2Fautowpscan%2F&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)


[pyversion-button]: https://img.shields.io/pypi/pyversions/Markdown.svg
[made-with-python]: https://img.shields.io/badge/Made%20with-Python-1f425f.svg


An automated tool that automatically scanning a list of multiple websites with wordpress at once. 

Requires wpscan.


## Introduction
This tool takes a list of multiple websites created with wordpress, lists them according to a predefined format, and uses wpscan to perform the scanning.

Nothing special, I created it because I needed automation. If you're good with code, I'm sure you can implement more sophisticated automation (e.g. Telegram bots, automatic checks on deployment via the Asset Information Report API, etc), or if you're thinking about your own DAST, this can help you with the initial development design. 

If you want to extend it further, you could create an administrative web UI and create self-service checks on the web UI, so that you can perform checks on demand.

## Requirements
- Wpscan must be installed on your system.
- Need a WordPress Vulnerability Database API token to analyze the results of the wpscan scan (you can get it from [here](https://wpscan.com/api))
- One or more websites developed with wordpress. 


## Features
- Multiprocessing to scan multiple websites at the same time.
- Send a summary of the scan results, logfile (in this tool, result will send to telegram, so you have to get a chat room)


## Limitations
It's important to note that this tool is not a replacement for manual testing, and it may not detect all vulnerabilities present in web applications. The tool should be used as a supplement to manual testing, and the results should be verified by a human tester before any action is taken. Additionally, the tool may produce false positives or false negatives, which should be considered when interpreting the results.

Overall, this tool can be a valuable addition to your web vulnerability testing process, helping you to identify and mitigate potential security risks in a large number of web applications.
