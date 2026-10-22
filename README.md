# Linux Practice Notes

Hands-on Linux practice for Cyber Security, using **OverTheWire: Bandit** and **SadServers**.

## Goal

- Build confident Linux command-line skills for SOC, security testing and troubleshooting work.
- Practise a clear investigation process: **observe → investigate → find root cause → fix → verify**.
- Support my preparation for the TryHackMe SAL1 certification and IT/Security internships.

## Platforms

| Platform | What I practise | Folder |
|---|---|---|
| [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) | Core commands, files, permissions, pipes, encoding, SSH | [`bandit/`](bandit/) |
| [SadServers](https://sadservers.com/) | Real-world troubleshooting: logs, processes, services, disk, network | [`sadservers/`](sadservers/) |

## Repository structure

```text
linux-practice-notes/
├── README.md
├── cheatsheet.md          # Commands I have actually used
├── bandit/
│   ├── README.md          # Progress tracker (no passwords, no spoilers)
│   └── concepts.md        # Notes organised by concept, not by level
└── sadservers/
    ├── README.md          # Progress tracker
    └── _template.md       # Write-up template
```

## Note on spoilers

OverTheWire asks players not to publish passwords or full solutions.
This repository only contains **concept notes and commands I learned**, not level passwords or step-by-step answers.

## Skills demonstrated

- Linux navigation, file handling and permissions
- Searching and filtering data with `find`, `grep`, `sort`, `uniq` and pipes
- Decoding and inspecting data (`base64`, `tr`, `xxd`, `strings`)
- Remote access with SSH and basic network services
- Structured troubleshooting and technical write-ups
