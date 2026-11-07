# AlekS ByeDPI for LG webOS — Public 0.6.32

**English** · [Русский](README_RU.md)

AlekS ByeDPI is a package for rooted LG webOS TVs with Homebrew Channel support. A local DNS/SNI bridge and native TCP processing help the **official YouTube application** connect under certain DPI filtering conditions. **It is not a VPN and does not guarantee connectivity on every network.**

## Features

- One IPK with ARMv7 and ARM64 native binaries and remote-control-friendly UI.
- Automatic LAN interface and private IPv4 detection (192.168.x.x, 10.x.x.x, 172.16–31.x.x); no hardcoded TV address.
- Separate local control and media SOCKS routes on ports 10881 and 10882.
- **R296:** bind DNS into the official YouTube Cobalt jail only after the native process is verified.
- Owned-process status monitoring, manual start/stop and restoration of modified networking settings.
- **No embedded private VPS IP addresses, telemetry sender, user tokens or private keys.**

## Installation

1. Use an authorized, rooted LG webOS device with Homebrew Channel and suitable LS2/ACG permissions.
2. Install com.gamefree24.byedpi_0.6.32_all.ipk using Homebrew or webOS SDK.
3. Open the app, select Enable ByeDPI and verify RUNNING.
4. Open official YouTube; test picture, sound and seeking.
5. If something fails, stop ByeDPI using its UI and revert using your saved old package.

**The IPK does not add persistent system startup hooks.** Following a cold boot you may need to restart YouTube or configure Homebrew separately. Keep a tested rollback package.

## Compatibility

The underlying private 0.6.31 version has user-confirmed playback on an LG 65NANO896PC with webOS 6.6. **The sanitized 0.6.32 Public candidate has NOT yet been tested on a physical TV.** LG 65UP7600LF and webOS 26 need separate testing. No universal hardware support guarantee.

## How it differs from generic ByeDPI

This package adds webOS/Homebrew/LS2 service integration, TV remote controls, automatic address discovery, Cobalt-jail-aware DNS/SNI handling, separate media and control paths, local diagnostics, and rollback. Performance depends on TV hardware, firmware and ISP.

## Privacy and licensing

No account or telemetry upload is required. The IPK still contains inspectable JavaScript, shell scripts and native binaries; **binary distribution does not prevent reverse engineering**.

© 2026 AlekS / GameFree24 for original AlekS components. Third-party licenses remain in force: hufrea ByeDPI MIT, hev MIT, musl MIT. See [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md) and the license texts included in the IPK. The unmodified binary package may be redistributed free of charge with attribution; this does not license all proprietary AlekS source code under MIT. Provided as-is without warranty.

For bug reports, provide the LG model, webOS version, build and symptoms. Do not share credentials, tokens, private keys or unredacted system logs.

**Checksum:** [SHA256SUMS.txt](SHA256SUMS.txt)