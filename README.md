# ar0x sherlock

<p align="center">
  <samp>ONE NAME. EVERY SITE. FOUND OR NOT.</samp>
</p>

A lightweight username reconnaissance tool built with **Bash + cURL**. Search across ~75 social platforms and discover publicly accessible profiles from a single terminal interface.

No Python. No package managers. No unnecessary dependencies.

---

## ◆ Features

- **~75 platforms** — Check popular social networks, developer communities, gaming platforms, and more.
- **Live hunt interface** — Animated banner, progress bar, counters, and real-time results.
- **Interactive verdict grid** — Watch every platform resolve as the hunt progresses.
- **Two detection methods** — HTTP status checks and page-content probes for platforms that return misleading status codes.
- **Parallel scanning** — Run up to 12 checks concurrently.
- **Profile navigation** — Browse discovered profiles and open them in your browser.
- **Exportable reports** — Save results for later analysis.
- **Persistent history** — Revisit your previous searches.
- **Terminal-friendly** — SSH support, ASCII fallback, and `NO_COLOR` compatibility.

## ◆ Quick start

### Requirements

- Bash 4+
- cURL
- A terminal

### Download and run

```bash
curl -fsSL https://raw.githubusercontent.com/ar0x1/ar0xsherlock/main/ar0xsherlock -o ar0xsherlock
chmod +x ar0xsherlock
./ar0xsherlock
```

Already cloned the repository? Run the script directly:

```bash
chmod +x ar0xsherlock
./ar0xsherlock
```

### Install as a command

```bash
mkdir -p ~/.local/bin
mv ar0xsherlock ~/.local/bin/ar0xsherlock
```

Ensure `~/.local/bin` is included in your `PATH`, then launch it from anywhere:

```bash
ar0xsherlock
```

Start a hunt immediately:

```bash
ar0xsherlock someuser
```

## ◆ The grid

Every platform receives a live verdict while the scan runs.

```text
╭─ ◆ THE GRID ─────────────────────────────────────╮
│                                                   │
│  ✓ GitHub    ✓ Reddit    ✓ Steam     ○ TikTok     │
│  ○ Twitch    – YouTube   – Medium    – Tumblr     │
│  ✗ Pinterest – Flickr    – Vimeo     – Genius     │
│                                                   │
│  ✓ found · ✗ blocked · – miss · ○ in flight       │
╰───────────────────────────────────────────────────╯
```

| Symbol | Verdict | Meaning |
|:---:|---|---|
| `✓` | Found | A matching profile was detected. |
| `–` | Miss | The platform indicated that the profile was absent. |
| `✗` | Blocked | The check failed or returned an inconclusive response. |
| `○` | In flight | The check is still running. |

Found profiles receive visual priority in the grid. Press `g` on the results screen to view the complete, scrollable grid with final verdicts for every checked platform.

*The grid above is a static illustration. Actual results depend on the username and each platform's response.*

## ◆ How the hunt works

ar0x sherlock uses two detection methods.

| Method | How it works | Typical use |
|---|---|---|
| `status` | Interprets HTTP status codes to determine whether a profile exists. | Most supported platforms |
| `probe` | Fetches the page and checks its content for indicators that the profile does not exist. | Platforms that return similar status codes for existing and missing profiles |

Checks run concurrently, with a browser-like User-Agent and a 10-second timeout per request.

During the hunt, the interface displays:

- Live progress and a progress bar
- Checked, found, missed, and blocked counters
- A real-time verdict feed
- Confirmed profiles as they are discovered

When the hunt finishes, browse the discovered profiles using the keyboard, open them in your browser, or export the results to a report.

## ◆ Keyboard controls

| Key | Action |
|---|---|
| `Enter` | Start the hunt or open the selected profile |
| `↑` / `↓` | Navigate through profiles or grid entries |
| `j` / `k` | Navigate using Vim-style keys |
| `g` | Open the full sweep grid |
| `s` | Save the report |
| `o` | Open the selected profile in your browser |
| `n` | Start a new hunt |
| `q` / `Esc` | Quit |
| `Ctrl+C` | Stop the hunt; retain partial results where supported |

Previous hunt history is stored in:

```text
~/.config/ar0xsherlock/
```

The interactive prompt can offer to repeat your previous hunt.

Reports are saved by default under `~/Downloads`, using a filename similar to:

```text
sherlock-<name>-<date>.txt
```

## ◆ Command-line usage

```bash
ar0xsherlock                 # Interactive mode
ar0xsherlock someuser        # Start with a username
ar0xsherlock -h              # Display help
ar0xsherlock -v              # Display version
```

## ◆ Scope & honesty

ar0x sherlock checks approximately 75 supported platforms. Coverage depends on the configured site list and the availability of each platform.

Some platforms, including Facebook, X, Instagram, and LinkedIn, are excluded because their anti-bot protections can prevent reliable username verification.

**A blocked check is not a negative result.** HTTP errors, timeouts, rate limits, and unusual responses can prevent a reliable verdict.

Likewise, a username that produces no matches is not necessarily available everywhere. A profile may be private, inaccessible, or hosted on an unsupported platform.

The tool reports what it can establish instead of pretending every result is certain.

> Built for research, username discovery, and checking your own digital footprint. Use it responsibly.

## ◆ Compatibility

| Requirement | Support |
|---|---|
| Shell | Bash 4+ |
| HTTP client | cURL |
| Linux | Supported |
| SSH terminals | Supported |
| Non-UTF-8 terminals | ASCII fallback |
| `NO_COLOR` | Respected |

The tool is designed to use only Bash and cURL, without Python or third-party package installations.

## ◆ Changelog

| Version | Changes |
|---|---|
| `1.0` | Initial hunt interface, terminal frames, and report support. |
| `1.1` | Added the live verdict grid and full sweep view (`g`). |
| `1.1.1` | Reworked the grid engine to avoid associative-array issues on Bash 4.2/4.3. |

## ◆ Credits

**Crafted by [ar0x](https://github.com/ar0x1)**, in the spirit of the original Sherlock project.

- **GitHub:** [github.com/ar0x1](https://github.com/ar0x1)
- **Email:** [killtoneizuku@gmail.com](mailto:killtoneizuku@gmail.com)

---

<p align="center">
  <samp>A NAME IS A TRAIL — FOLLOW IT.</samp>
</p>
