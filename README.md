# `ar0xsherlock`

<p align="center">
  <b>Hunt usernames. Follow the public trail.</b>
</p>

<p align="center">
  A lightweight username OSINT tool built with Bash and cURL.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.1.1-00D4AA?style=flat-square" />
  <img src="https://img.shields.io/badge/language-Bash-121212?style=flat-square&logo=gnubash&logoColor=white" />
  <img src="https://img.shields.io/badge/engine-cURL-121212?style=flat-square&logo=curl&logoColor=white" />
  <img src="https://img.shields.io/badge/platform-Linux-121212?style=flat-square&logo=linux&logoColor=white" />
</p>

---

## ◈ Overview

**ar0xsherlock** is a terminal-based username discovery tool that checks usernames across multiple websites and services.

Built with Bash and cURL, it combines concurrent HTTP requests with an interactive terminal interface to make public-profile discovery simple and efficient.

## ◈ Features

- **Multi-site scanning** — Check usernames across supported websites.
- **Concurrent requests** — Scan multiple services simultaneously.
- **Interactive terminal UI** — A clean, colorful CLI experience.
- **Live results** — Follow scan progress directly in your terminal.
- **Lightweight** — Powered by Bash and cURL.
- **Quick launch** — Install and run with a single command.

## ◈ Installation

### Quick Install

Copy and paste this command into your terminal:

```bash
curl -fsSL https://raw.githubusercontent.com/ar0x1/arl0x/main/ar0xsherlock -o ar0xsherlock && chmod +x ar0xsherlock && ./ar0xsherlock
```

This downloads the script, makes it executable, and launches the tool.

**Note:** Replace `YOUR_USERNAME` with your GitHub username. This command assumes the script is named `ar0xsherlock` and is located in the repository's `main` branch root.

### Manual Installation

```bash
git clone https://github.com/ar0x1/arl0x.git
cd ar0xsherlock
chmod +x ar0xsherlock
./ar0xsherlock
```

## ◈ Usage

**Interactive mode**

```bash
./ar0xsherlock
```

**Search a specific username**

```bash
./ar0xsherlock username
```

**Show help**

```bash
./ar0xsherlock --help
```

**Show version**

```bash
./ar0xsherlock --version
```

## ◈ Requirements

- Linux or a compatible Unix-like environment
- Bash 4+
- cURL
- Internet connection
- Interactive terminal

## ◈ How It Works

1. Accepts a target username.
2. Checks supported websites using profile URLs.
3. Sends HTTP requests through cURL.
4. Processes responses and displays potential profile matches.
5. Presents results directly in the terminal.

Detection accuracy depends on website response behavior, redirects, rate limits, and network conditions. Results should be independently verified when necessary.

## ◈ Responsible Use

- Use the tool for legitimate OSINT and public-profile research.
- Respect website terms of service and privacy.
- Follow applicable laws.
- Do not use discovered information to harass or harm others.

## ◈ Disclaimer

This tool is provided for educational and legitimate research purposes. The developer is not responsible for misuse or decisions made based on scan results.

## ◈ Contributing

Contributions, bug reports, and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Submit a pull request.
## ◈ Author

Created by **ar0x** · [GitHub profile](https://github.com/ar0x1) · [Contact](killtoneizuku@gmail.com)

---

<p align="center">
  <b>ar0xsherlock</b><br>
  <sub>Find the handle. Follow the public trail.</sub>
</p>
