# `ar0xsherlock`

<p align="center">
  <b>Hunt usernames. Discover profiles. Stay in the terminal.</b>
</p>

<p align="center">
  A lightweight, terminal-based username OSINT tool built with Bash and cURL.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.1.1-00D4AA?style=flat-square" />
  <img src="https://img.shields.io/badge/language-Bash-121212?style=flat-square&logo=gnubash&logoColor=white" />
  <img src="https://img.shields.io/badge/engine-cURL-121212?style=flat-square&logo=curl&logoColor=white" />
  <img src="https://img.shields.io/badge/platform-Linux-121212?style=flat-square&logo=linux&logoColor=white" />
</p>

---

## ◈ Overview

**`ar0xsherlock`** is a command-line username discovery tool that checks a username across multiple websites and services.

Built for terminal lovers, it combines a clean interactive interface with concurrent HTTP requests to make public-profile discovery simple and efficient.

No heavy framework. No unnecessary dependencies. Just Bash, cURL, and the terminal.

## ◈ Features

- **Multi-site scanning** — Check usernames across dozens of websites.
- **Concurrent requests** — Scan multiple services at once.
- **Interactive terminal UI** — A colorful, organized scanning interface.
- **Live results** — Watch the scan progress in real time.
- **Profile links** — Identify matching public profiles.
- **Lightweight** — Built with Bash and cURL.
- **Simple usage** — Launch interactively or provide a username directly.

## ◈ Preview

```text
       ▄▀█ █▀█ █▀█ ▀█▀ █ █ █▀█ █▀▀ █▀█ █   █▀█ █▀▀ █▀█
       █▀█ █▀▄ █▄█  █  █▄█ █▀▄ ██▄ █▀▄ █▄▄ █▄█ █▄▄ █▀▄

       ┌────────────────────────────────────────┐
       │         ar0xsherlock  v1.1.1            │
       │     Username Intelligence Scanner      │
       └────────────────────────────────────────┘

       [ + ] Target     : username
       [ + ] Engine     : Bash + cURL
       [ + ] Mode       : Multi-site scan

       [ * ] Scanning public profiles...
       [ + ] Profile found
       [ - ] No profile detected
```

*Illustrative terminal preview; actual output may differ.*

## ◈ Requirements

- Linux or another Unix-like environment
- Bash 4+
- cURL
- An interactive terminal
- Internet connection

## ◈ Installation

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/ar0xsherlock.git
cd ar0xsherlock
```

Make the script executable:

```bash
chmod +x ar0xsherlock
```

Run it:

```bash
./ar0xsherlock
```

Replace `YOUR_USERNAME` with your actual GitHub username.

## ◈ Usage

**Interactive mode**

```bash
./ar0xsherlock
```

Launch the tool and enter the username when prompted.

**Direct scan**

```bash
./ar0xsherlock username
```

Replace `username` with the public username you want to check.

**Show help**

```bash
./ar0xsherlock --help
```

**Show version**

```bash
./ar0xsherlock --version
```

## ◈ How It Works

1. Accepts a target username.
2. Builds profile URLs for supported websites.
3. Sends HTTP requests using cURL.
4. Processes responses to determine whether a profile appears to exist.
5. Displays the results in the terminal.

Results depend on each website's response behavior. Redirects, rate limits, network errors, login requirements, and changes to website layouts can affect detection accuracy.

## ◈ Compatibility

The tool is designed for Bash 4+ environments with cURL installed. Some websites may block automated requests or return ambiguous responses, so results should be verified when accuracy matters.

## ◈ Responsible Use

`ar0xsherlock` is intended for legitimate OSINT, username discovery, and public-profile research.

- Respect website terms of service.
- Follow applicable laws and privacy rules.
- Avoid harassment, unauthorized access, and misuse of discovered information.
- Treat scan results as indicators, not guaranteed proof of identity.

## ◈ Disclaimer

This project is provided for educational and legitimate research purposes. The developer is not responsible for misuse of this tool or for decisions made based on its results.

## ◈ Contributing

Contributions, bug reports, and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Submit a pull request.

## ◈ License

Add your chosen license file and update this section accordingly.

---

<p align="center">
  <b>ar0xsherlock</b><br>
  <sub>Find the handle. Follow the public trail.</sub>
</p>
