# `ar0xsherlock`

<p align="center">
  <b>ONE NAME. EVERY SITE. FIND THE PUBLIC TRAIL.</b>
</p>

<p align="center">
  A terminal-based username OSINT tool built with Bash and cURL.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.1.1-00D4AA?style=flat-square" />
  <img src="https://img.shields.io/badge/Bash-4%2B-121212?style=flat-square&logo=gnubash&logoColor=white" />
  <img src="https://img.shields.io/badge/cURL-powered-121212?style=flat-square&logo=curl&logoColor=white" />
  <img src="https://img.shields.io/badge/Platform-Linux-121212?style=flat-square&logo=linux&logoColor=white" />
</p>

---

## ◈ About

**ar0xsherlock** is a lightweight username discovery tool that checks public profile URLs across approximately 75 popular websites.

Built entirely with Bash and cURL, it features concurrent scanning, a live terminal grid, profile browsing, and report generation.

## ◈ Features

- **Multi-site scanning** — Check usernames across supported websites.
- **Live terminal grid** — Follow scan results as they arrive.
- **Concurrent requests** — Check multiple websites in parallel.
- **Profile browser** — Open discovered profile links.
- **Report generation** — Save scan reports to your Downloads directory.
- **Scan history** — Remember previously searched usernames.
- **Lightweight** — Bash and cURL, without a heavy framework.
- **Color-aware UI** — Terminal colors with a `NO_COLOR` fallback.

## ◈ Quick Start

### One-command launch


This downloads the script and launches it directly in Bash without saving a separate script file.

Copy and paste this into your terminal:

### Download and install

```bash
curl -fsSL https://raw.githubusercontent.com/ar0x1/ar0xsherlock/main/arr0xsherlock.txt -o ar0xsherlock
chmod +x ar0xsherlock
./ar0xsherlock
```

## ◈ Requirements

- Linux or a compatible Unix-like environment
- Bash 4 or newer
- cURL
- Internet connection
- Interactive terminal

Install cURL if needed:

**Debian / Ubuntu / Kali Linux**

```bash
sudo apt update && sudo apt install curl
```

**Fedora**

```bash
sudo dnf install curl
```

**Arch Linux**

```bash
sudo pacman -S curl
```

## ◈ Usage

Launch the interactive interface:

```bash
./ar0xsherlock
```

Start with a username already entered:

```bash
./ar0xsherlock username
```

Show help:

```bash
./ar0xsherlock --help
```

Show version:

```bash
./ar0xsherlock --version
```

Usernames must be 2–32 characters and may contain letters, numbers, dots, underscores, and hyphens.

## ◈ Terminal Controls

| Key | Action |
|---|---|
| `↑` / `↓` or `j` / `k` | Navigate results |
| `Enter` / `o` | Open the selected profile |
| `g` | Open the scan grid |
| `s` | Save a report |
| `n` | Search another username |
| `q` | Quit or return |

## ◈ How It Works

1. Enter a username.
2. The tool checks supported profile URLs using cURL.
3. Requests run concurrently, with a timeout for individual checks.
4. Results are displayed in the terminal grid.
5. Browse discovered profiles or save a report.

A website marked as blocked or returning an unexpected response does not necessarily mean the profile is absent.

## ◈ Limitations

- Some websites block automated requests.
- Rate limits, redirects, and network issues can affect results.
- A detected profile does not prove that it belongs to a particular person.
- Results should be independently verified.

## ◈ Responsible Use

Use this tool for legitimate OSINT and public-profile research. Respect website terms of service, privacy, and applicable laws. Do not use the results to harass, impersonate, or harm others.

## ◈ Disclaimer

This project is provided for educational and legitimate research purposes. Use it responsibly and verify important findings independently.

## ◈ Author

**ar0x**

- GitHub: [@ar0x1](https://github.com/ar0x1)
- Contact: `killtoneizuku@gmail.com`

## ◈ License

Refer to the repository's license file, if provided.

---

<p align="center">
  <b>ar0xsherlock</b><br>
  <sub>Find the handle. Follow the public trail.</sub>
</p>
