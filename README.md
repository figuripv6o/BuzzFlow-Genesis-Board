# PulseScan

PulseScan is a lightweight, paste-safe network discovery utility designed for
Termux and constrained environments.

It performs fast TCP reachability checks across CIDR ranges with predictable,
structured output and optional JSON emission.

---

## Features

- CIDR, IP-range, or file-based targets
- Safe View mode (text-only, paste-safe output)
- Structured JSON status output
- Deterministic defaults (no surprises)
- No color, no ANSI, no binary leakage
- Termux-compatible

---

## Usage

pulsescan --target <CIDR|IP-range|file> [options]

### Required
--target <CIDR|IP-range|file>
    Network scope to scan.
    Examples:
      127.0.0.1/32
      192.168.1.1-192.168.1.254
      targets.txt

### Optional
--ports <list>
    Comma-separated ports.
    Default: 80,443

--rate <pps>
    Probe rate in packets per second.

--timeout <ms>
    Probe timeout in milliseconds.

--emit-binary <file>
    Write raw scan artifact to file (no stdout).

--status-json <file>
    Emit structured JSON status output.

--safe-view
    Text-only output. No control characters. Paste-safe.

--quiet
