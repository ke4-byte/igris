Markdown
# ⚽ Bot Igris & Squad Management Engine

A Python-powered automation tool and player database management system. It provides rate-limited social API automation compliant with safety thresholds and automates player/squad data tracking via Google Sheets and Google Calendar.

## 🛠️ Features

* **Rate-Limited Automation:** Enforces strict hourly caps, pacing delays, and a 48-hour circuit breaker on API errors.
* **Autonomous Scheduling:** Integrates with **Google Calendar API** to distribute execution batches evenly across natural daily time windows.
* **Player Database Integration:** Reads and writes player stats, authentication profiles, and team roles via **Google Sheets**.
* **Desktop GUI Interface:** Built with `pywebview` for easy tracking, event logging, and execution control.


## 🚀 Quick Start

### 1. Prerequisites
Ensure you have Python 3.9 or higher installed.

```bash
python --version


2. Installation
Clone the repository and install the dependencies:

Bash
git clone [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git)
cd YOUR_REPO_NAME
pip install -r requirements.txt



🖥️ Usage
Run the GUI Application
Launch the desktop interface to manage schedules, view logs, and run execution batches:


Bash
python gui.py


Run via Command Line / Core Engine
To trigger the underlying execution engine directly:


Bash
python igris_engine.py


📋 Recommended Operational Flow
Import / Load Data: Connect your Google Sheet containing player and account information.
Generate Schedule: Run the calendar sync to push execution slots to Google Calendar.
Execute Engine: Start the automation batcher.
Monitor Logs: Track active delays, session targets, and API responses directly from the console or GUI tab.
🛡️ Rate Limits & Safety Compliance
Account Age
Max Daily Actions
Hourly Cap
Pacing Delay
New (< 6 Months)
80 / day
10–15 / hr
180s – 300s
Established (> 6 Months)
150 / day
20–30 / hr
120s – 180s

📄 License
This project is licensed under my License.
