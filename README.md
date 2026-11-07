# AlekS ByeDPI for LG webOS — Public 0.6.32

**[Русская инструкция](README_RU.md) · [English README](README_EN.md)**

A privacy-reduced, binary-only public **beta** build for rooted LG webOS televisions.

- Includes R656 local DNS/SNI controller, R296 Cobalt DNS late-binding, automatic private LAN IPv4 detection and ARMv7/ARM64 binaries.
- Removes embedded private VPS addresses and all optional telemetry code.
- **No hardware playback verification yet for this specific 0.6.32 build.** The underlying private 0.6.31 worked on the developer's hall TV; this is not the same installed binary.
- Root + Homebrew Channel are required. No automatic boot hook is installed.
- All package checksums are in [SHA256SUMS.txt](SHA256SUMS.txt).

The distribution archive contains inspectable JavaScript and shell scripts. It is not proof against reverse engineering; only the sanitized public edition is intended for sharing.

Read the [release notes](RELEASE_NOTES.md), [security policy](SECURITY.md), and [third-party notices](THIRD_PARTY_NOTICES.md) before installation.
