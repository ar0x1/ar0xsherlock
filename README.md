# `ar0xsherlock`

<p align="center">
  <b>USERNAME RECONNAISSANCE · STRAIGHT FROM YOUR TERMINAL</b>
</p>

<p align="center">
  A lightweight Bash and cURL tool for discovering public profiles across multiple websites.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.1.1-00D4AA?style=flat-square" />
  <img src="https://img.shields.io/badge/Bash-4%2B-121212?style=flat-square&logo=gnubash&logoColor=white" />
  <img src="https://img.shields.io/badge/Powered%20by-cURL-121212?style=flat-square&logo=curl&logoColor=white" />
</p>

---

## ◈ Features

- Multi-site username scanning
- Concurrent HTTP requests
- Interactive terminal interface
- Live scan progress and results
- Lightweight Bash implementation
- Simple command-line usage

## ◈ Installation

### Requirements

- Linux or a compatible Unix-like system
- Bash 4+
- cURL
- Git
- Internet connection

### Quick Start

```bash
bash <(curl -fsSL https://raw.githubusercontent.com/ar0x1/ar0xsherlok/main/ar0xsherlock)
```
OR

Copy and paste the following commands into your terminal:

```bash
git clone https://github.com/ar0x1/ar0xsherlok.git
cd ar0xsherlok
ls -la
```

Make sure the main script is named `ar0xsherlock`. Then run:

```bash
chmod +x ar0xsherlock
./ar0xsherlock
```

If the script is not executable or you prefer to launch it through Bash:

```bash
bash ./ar0xsherlock
```

**Important:** If `ls -la` shows a different script filename, use that exact filename in the commands above.

## ◈ Usage

Launch the interactive interface:

```bash
./ar0xsherlock
```

Search for a username:

```bash
./ar0xsherlock username
```

Display help:

```bash
./ar0xsherlock --help
```

Display version:

```bash
./ar0xsherlock --version
```

Replace `username` with the handle you want to check.

## ◈ How It Works

1. Accepts a username as input.
2. Checks supported websites using HTTP requests.
3. Processes the responses.
4. Displays potential public-profile matches in the terminal.

Website changes, rate limits, redirects, and network failures can affect detection accuracy.

## ◈ Responsible Use

Use `ar0xsherlock` for legitimate OSINT and public-profile research. Respect website terms, applicable laws, and individual privacy. Do not use discovered information to harass or harm others.

## ◈ Disclaimer

This project is provided for educational and legitimate research purposes. Results are indicators, not guaranteed proof of identity. Use the tool responsibly.

## ◈ Contributing

Bug reports, suggestions, and pull requests are welcome.
## ◈ Author

Created by **ar0x** · [GitHub profile](https://github.com/ar0x1) · [Contact](killtoneizuku@gmail.com)

---

<p align="center">
  <b>ar0xsherlock</b><br>
  <sub>Find the handle. Follow the public trail.</sub>
</p>
