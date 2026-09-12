<div align="center">

🚀 INDIA SERVER SCRAPER

⚡ Fast • Async • Protected • Cross-Platform IPTV/Xtream Live TV Checker

<a href="https://github.com/">
  <img src="https://img.shields.io/badge/Python-3.9%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
</a>
<a href="https://github.com/">
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20Linux%20%7C%20Termux-111827?style=for-the-badge" alt="Platform">
</a>
<a href="https://github.com/">
  <img src="https://img.shields.io/badge/Mode-Async-00A67D?style=for-the-badge" alt="Async">
</a>
<a href="https://github.com/">
  <img src="https://img.shields.io/badge/Status-Ready-22C55E?style=for-the-badge" alt="Status">
</a>

<br><br>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=22&duration=2200&pause=700&color=00F0FF&center=true&vCenter=true&width=850&lines=INDIA+SERVER+SCRAPER;Async+Xtream%2FXUI+Live+TV+Checker;M3U8+%2B+TS+Stream+Verification;Windows+%7C+Linux+%7C+Termux;Protected+Build+by+Subroto+Roy" alt="Typing animation">

<br>

Developer: @Krishna_Subroto

</div>

✨ Overview

INDIA SERVER SCRAPER is an asynchronous Python-based Xtream/XUI-compatible Live TV checker.

It connects to an authorized IPTV/Xtream server, authenticates with the supplied credentials, loads live-TV categories and channels, verifies returned streams, and writes verified working channels into an M3U playlist.

🔐 Use only servers, accounts and streams that you are authorized to access.

🌟 Main Features

Feature

Description

🚀 Async Scanner

Concurrent stream checking using asyncio + aiohttp

🔐 Authentication

Xtream/XUI-style API login

📺 Live TV Fetch

Fetches all returned live-TV entries

🗂️ Categories

Loads live categories when available

✅ Stream Verification

Checks M3U8/HLS and MPEG-TS responses

🔄 Retry

Retries failed stream checks according to configuration

⚡ Concurrency

Multiple stream checks at the same time

📦 Batch Processing

Large channel lists are processed in batches

📄 M3U Export

Saves only verified working streams

🛡️ Protected Build

Protected version includes integrity/protection logic

💻 Cross Platform

Windows, Linux and Termux

📁 Project Structure

.
├── india_server_scraper.py
├── requirements.txt
├── README.md
└── working_channels.m3u

working_channels.m3u is generated automatically after a successful scan.

🛠️ Installation

🪟 Windows

1. Install Python

Install Python 3.9 or newer and make sure Python is added to PATH.

Check:

python --version

or:

py --version

2. Open the project folder

cd path\to\your\project

3. Install dependencies

python -m pip install -r requirements.txt

4. Run

python india_server_scraper.py

If your system uses the py launcher:

py india_server_scraper.py

🐧 Linux

1. Check Python

python3 --version

2. Install pip if required

Ubuntu/Debian:

sudo apt update
sudo apt install python3 python3-pip

3. Open the project directory

cd /path/to/project

4. Install requirements

python3 -m pip install -r requirements.txt

If your distribution requires an external managed environment, create a virtual environment:

python3 -m venv venv
source venv/bin/activate
python3 -m pip install -r requirements.txt

5. Run

python3 india_server_scraper.py

📱 Termux

1. Update packages

pkg update && pkg upgrade

2. Install Python

pkg install python

Check:

python --version

3. Go to the project folder

Example:

cd ~/india-server-scraper

4. Install requirements

pip install -r requirements.txt

5. Run

python india_server_scraper.py

📂 Optional: access phone storage

termux-setup-storage

Then you can work from a folder under:

~/storage/

📦 Requirements

requirements.txt:

aiohttp
cryptography

The protected build uses Python standard-library modules as well, so those do not need separate installation.

▶️ Usage

When the program starts, it asks for:

[1] Host Name :
[2] Username  :
[3] Password  :

Example format:

Host Name : http://example.com:8080
Username  : your_username
Password  : your_password

The password is entered as hidden input.

The normal flow is:

┌──────────────────────┐
│  Enter Server Data   │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│   API Authentication │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│  Load Live Categories│
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Fetch Live TV Entries│
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Verify M3U8 / TS URL │
└──────────┬───────────┘
           ↓
┌──────────────────────┐
│ Save Working Streams │
└──────────┬───────────┘
           ↓
    working_channels.m3u

📺 Output

After scanning, the program creates:

working_channels.m3u

The playlist contains only streams that passed the verification checks.

Example:

#EXTM3U
#EXTINF:-1 tvg-id="123" tvg-name="Example Channel" tvg-logo="" group-title="Live TV",Example Channel
http://example.com/live/user/pass/123.m3u8

⚙️ Configuration

The main scanner settings are kept inside the Python program.

Typical settings include:

MAX_CONCURRENCY = 80
BATCH_SIZE = 500
API_TIMEOUT = 20
STREAM_TIMEOUT = 12
RETRY_COUNT = 1
MAX_REDIRECTS = 5
VERIFY_BYTES = 4096

What they control

MAX_CONCURRENCY → maximum simultaneous stream checks

BATCH_SIZE → number of channels processed per batch

API_TIMEOUT → API request timeout

STREAM_TIMEOUT → stream verification timeout

RETRY_COUNT → retry count for failed stream checks

MAX_REDIRECTS → allowed HTTP redirects

VERIFY_BYTES → bytes inspected during stream verification

⚠️ Increase concurrency carefully. Very high values can increase CPU, RAM, bandwidth usage, server load, or trigger remote rate limits.

🛡️ Protected Build

The protected version is intended to make casual source inspection and modification more difficult while preserving the program's normal runtime behavior.

Important

No Python .py file can be made 100% impossible to reverse engineer or modify once another person has the file and can execute it.

Protection should therefore be treated as:

Source hiding + integrity checking + harder casual editing

—not as an absolute cryptographic guarantee.

🧪 Troubleshooting

ModuleNotFoundError: No module named 'aiohttp'

Run:

python -m pip install -r requirements.txt

On Linux/Termux:

python3 -m pip install -r requirements.txt

or:

pip install -r requirements.txt

Python command not found

Windows:

py --version

Linux:

python3 --version

Termux:

python --version

Server authentication fails

Check that:

Host
Username
Password

are correct and that you are authorized to use the server.

Also verify that the server exposes a compatible Xtream/XUI API.

0 live channels returned

Possible causes include:

The account has no live-TV entries.

The server API returned an unexpected response.

The credentials have limited permissions.

The panel is not compatible with the expected API format.

Streams show as dead

A stream can fail verification because of:

network problems

expired credentials

unavailable stream

invalid stream endpoint

remote server timeout

unsupported response format

🔒 Security Notes

Never publish real credentials in:

GitHub commits

screenshots

README files

issue trackers

public Telegram groups

public paste sites

Use only authorized IPTV/Xtream servers and accounts.

⚡ Performance Tips

For large channel lists:

BATCH_SIZE       → controls batch processing
MAX_CONCURRENCY  → controls simultaneous checks
STREAM_TIMEOUT   → controls per-stream waiting time
RETRY_COUNT      → controls retry behavior

A faster configuration is not always better. Your network, VPS/phone hardware, and remote server limits all matter.

🖥️ Supported Platforms

<div align="center">

Platform

Supported

🪟 Windows

✅

🐧 Linux

✅

📱 Termux

✅

💻 VPS

✅

☁️ Cloud Linux

✅

</div>

📜 Disclaimer

This project is intended for authorized testing, administration and verification of IPTV/Xtream-compatible servers and accounts.

The developer does not provide or authorize unauthorized access to third-party systems.

You are responsible for how you use this software and for ensuring that your activity complies with applicable laws, service terms and the authorization of the server owner.

<div align="center">

💙 Developed by

@Krishna_Subroto

⚡ INDIA SERVER SCRAPER

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00F0FF,100:7C3AED&height=120&section=footer" alt="Footer animation">

</div>
