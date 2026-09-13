<div align="center">

🚀 INDIA SERVER SCRAPER

⚡ Async Xtream/XUI Live TV Checker • M3U8 / TS Verification







<br>

<a href="https://t.me/Krishna_Subroto">
<img src="https://img.shields.io/badge/Developer-@Krishna__Subroto-229ED9?style=for-the-badge&logo=telegram&logoColor=white" alt="@Krishna_Subroto">
</a>
<a href="https://t.me/i_stay_silent_not_week">
<img src="https://img.shields.io/badge/Developer-@i__stay__silent__not__week-229ED9?style=for-the-badge&logo=telegram&logoColor=white" alt="@i_stay_silent_not_week">
</a>

<br><br>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=800&size=24&duration=2200&pause=700&color=00E5FF&center=true&vCenter=true&width=900&lines=INDIA+SERVER+SCRAPER;FAST+ASYNC+LIVE+TV+CHECKER;M3U8+%2B+TS+STREAM+VERIFICATION;WINDOWS+%7C+LINUX+%7C+TERMUX;PROTECTED+BUILD;AUTHORIZED+USE+ONLY" alt="Animated title">

<br>

🔥 Professional • Fast • Lightweight • Cross-Platform

</div>

🌟 About

INDIA SERVER SCRAPER is an asynchronous Python tool for checking authorized Xtream/XUI-compatible Live TV servers.

The program:

HOST
  ↓
USERNAME
  ↓
PASSWORD
  ↓
API AUTHENTICATION
  ↓
FETCH LIVE TV
  ↓
CHECK M3U8 / TS STREAMS
  ↓
FILTER WORKING CHANNELS
  ↓
SAVE working_channels.m3u

It is designed to work on:

🪟 Windows

🐧 Linux

📱 Termux

☁️ Linux VPS

🔐 Only use servers, accounts and streams that you are authorized to access.

✨ Features

Feature

Details

🚀 Async checking

Uses asynchronous requests for concurrent verification

🔐 API authentication

Xtream/XUI-style authentication

📺 Live TV fetching

Retrieves available live-TV entries

🗂️ Categories

Loads live categories when supported

✅ M3U8 verification

Detects HLS playlist responses

✅ TS verification

Checks MPEG-TS stream signatures

🔄 Retry support

Failed checks can be retried

⚡ Concurrent workers

Multiple channels checked at once

📦 Batch processing

Large channel lists processed in batches

📄 M3U export

Working streams saved automatically

🛡️ Protected build

Includes source-protection / integrity logic

💻 Cross-platform

Windows + Linux + Termux

📁 Project Files

india-server-scraper/
│
├── india_server_scraper.py
├── requirements.txt
├── README.md
│
└── working_channels.m3u
       └── generated after a successful scan

india_server_scraper.py

Main application file.

requirements.txt

Required Python package list.

README.md

This documentation.

working_channels.m3u

Automatically generated output containing verified channels.

📦 Requirements

Python

Recommended:

Python 3.9+

Check your version:

python --version

Linux users can also use:

python3 --version

🪟 WINDOWS

1️⃣ Install Python

Install Python 3.9+ from the official Python website.

During installation, enable:

☑ Add Python to PATH

Verify:

python --version

or:

py --version

2️⃣ Open the project directory

Example:

cd C:\Users\YourName\Desktop\india-server-scraper

3️⃣ Install dependencies

python -m pip install -r requirements.txt

If your computer uses py:

py -m pip install -r requirements.txt

4️⃣ Start the scraper

python india_server_scraper.py

or:

py india_server_scraper.py

🪟 Windows Quick Start

cd C:\path\to\project
python -m pip install -r requirements.txt
python india_server_scraper.py

🐧 LINUX

1️⃣ Check Python

python3 --version

2️⃣ Install Python and pip

Ubuntu / Debian

sudo apt update
sudo apt install python3 python3-pip

3️⃣ Open the project directory

cd /path/to/india-server-scraper

4️⃣ Install dependencies

python3 -m pip install -r requirements.txt

Recommended: virtual environment

python3 -m venv venv
source venv/bin/activate
python3 -m pip install -r requirements.txt

5️⃣ Run

python3 india_server_scraper.py

🐧 Linux Quick Start

sudo apt update
sudo apt install python3 python3-pip
cd /path/to/project
python3 -m pip install -r requirements.txt
python3 india_server_scraper.py

📱 TERMUX

1️⃣ Update Termux

pkg update && pkg upgrade

2️⃣ Install Python

pkg install python

Verify:

python --version

3️⃣ Open your project folder

Example:

cd ~/india-server-scraper

4️⃣ Install dependencies

pip install -r requirements.txt

5️⃣ Run

python india_server_scraper.py

📂 Optional: Termux Storage

To access your phone storage:

termux-setup-storage

Then you can access:

~/storage/shared/

For example:

cd ~/storage/shared/india-server-scraper
python india_server_scraper.py

📱 Termux Quick Start

pkg update && pkg upgrade
pkg install python
cd ~/india-server-scraper
pip install -r requirements.txt
python india_server_scraper.py

📄 REQUIREMENTS.TXT

The recommended requirements.txt is:

aiohttp

The Python standard library modules used by the application do not need to be installed separately.

Install everything with:

pip install -r requirements.txt

▶️ HOW TO USE

Start the program:

python india_server_scraper.py

The program will ask for:

[1] Host Name :
[2] Username  :
[3] Password  :

Example:

[1] Host Name : http://example.com:8080
[2] Username  : your_username
[3] Password  : your_password

The password is entered using hidden input.

🔄 SCAN FLOW

╔══════════════════════════════════════╗
║         INDIA SERVER SCRAPER         ║
╚══════════════════╦═══════════════════╝
                   ║
                   ▼
        ┌─────────────────────┐
        │ Enter Server Details│
        └──────────┬──────────┘
                   ▼
        ┌─────────────────────┐
        │    Authentication   │
        └──────────┬──────────┘
                   ▼
        ┌─────────────────────┐
        │  Load Categories    │
        └──────────┬──────────┘
                   ▼
        ┌─────────────────────┐
        │ Fetch Live TV List  │
        └──────────┬──────────┘
                   ▼
        ┌─────────────────────┐
        │  Verify M3U8 / TS   │
        └──────────┬──────────┘
                   ▼
        ┌─────────────────────┐
        │ Keep Working Streams│
        └──────────┬──────────┘
                   ▼
        ┌─────────────────────┐
        │ working_channels.m3u│
        └─────────────────────┘

⚙️ CONFIGURATION

The scanner contains configuration values for performance and timeout handling.

Typical settings include:

MAX_CONCURRENCY = 80
BATCH_SIZE = 500
API_TIMEOUT = 20
STREAM_TIMEOUT = 12
RETRY_COUNT = 1
MAX_REDIRECTS = 5
VERIFY_BYTES = 4096

🔥 What they do

MAX_CONCURRENCY

Controls how many stream checks can run at the same time.

BATCH_SIZE

Prevents very large server lists from creating too many tasks at once.

API_TIMEOUT

Controls API request timeout.

STREAM_TIMEOUT

Controls how long a stream check can wait.

RETRY_COUNT

Controls retry attempts.

MAX_REDIRECTS

Controls the maximum allowed redirects.

VERIFY_BYTES

Controls how much stream data is inspected during verification.

⚠️ Do not blindly increase concurrency. Remote server limits, network bandwidth, RAM and CPU all affect performance.

🛡️ PROTECTED BUILD

The protected version is intended to make casual source inspection and straightforward editing more difficult while retaining normal runtime behavior.

Typical protected workflow:

Original Application
        ↓
Protection / Packaging
        ↓
Protected Python File
        ↓
Runtime Integrity Check
        ↓
Application Starts

⚠️ Important

No Python .py file can be made mathematically impossible to reverse-engineer once someone has the executable/source artifact and enough control over the runtime environment.

The protection goal is:

✅ Harder to casually inspect
✅ Harder to casually edit
✅ Detect modified payloads
✅ Keep normal execution working

—not an absolute guarantee against reverse engineering.

🔧 REPLACING THE PROTECTED FILE

If you receive an updated protected build, replace the old Python file with the new file while keeping:

requirements.txt
README.md

and your output location intact.

Then reinstall requirements if necessary:

pip install -r requirements.txt

and run:

python india_server_scraper.py

📄 OUTPUT

After a successful scan, the program writes:

working_channels.m3u

The file contains:

#EXTM3U

followed by verified channel entries.

Example structure:

#EXTM3U
#EXTINF:-1 tvg-id="123" tvg-name="Example Channel" tvg-logo="" group-title="Live TV",Example Channel
http://example.com/live/user/pass/123.m3u8

You can then import the M3U playlist into a compatible IPTV player.

🧪 TROUBLESHOOTING

❌ No module named 'aiohttp'

Run:

python -m pip install -r requirements.txt

Linux:

python3 -m pip install -r requirements.txt

Termux:

pip install -r requirements.txt

❌ python command not found

Windows

Try:

py --version

Linux

Try:

python3 --version

Termux

Try:

pkg install python
python --version

❌ Authentication failed

Verify:

Host
Username
Password

and make sure the account is authorized and compatible with the expected API.

❌ 0 live channels

Possible reasons:

• Account has no Live TV entries
• API returned an unexpected response
• Account permissions are limited
• Server does not support the expected API format

❌ All streams appear dead

Possible reasons:

• Network issue
• Remote server timeout
• Expired credentials
• Invalid stream endpoints
• Unsupported response type
• Server rate limiting

🔐 SECURITY

Never put real credentials inside:

README.md
GitHub issues
Public commits
Screenshots
Public Telegram messages
Paste sites

Always remove or hide credentials before publishing logs or screenshots.

🎯 SUPPORTED ENVIRONMENTS

Environment

Status

🪟 Windows

✅

🐧 Linux

✅

📱 Termux

✅

☁️ VPS

✅

🖥️ Linux Server

✅

💻 Desktop Python

✅

📌 DEVELOPER

<div align="center">

👨‍💻 Developers

<a href="https://t.me/Krishna_Subroto">



</a>

<a href="https://t.me/i_stay_silent_not_week">



</a>

<br>

Built with ❤️ • Python • asyncio • aiohttp

</div>

⚖️ DISCLAIMER

This software is intended for authorized testing, administration and verification of IPTV/Xtream-compatible servers and accounts.

Use only systems and accounts you have permission to access.

The user is responsible for complying with applicable laws, contracts, service terms and the server owner's authorization.

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00E5FF,50:2563EB,100:7C3AED&height=180&section=footer&text=INDIA%20SERVER%20SCRAPER&fontSize=28&fontColor=ffffff&animation=fadeIn" alt="Animated footer">

⭐ INDIA SERVER SCRAPER ⭐

Developed by @Krishna_Subroto & @i_stay_silent_not_week

</div>
