# AlekS ByeDPI 0.6.34 — R327 diagnostic beta

**Isolated test release**, not the main feed. It adds bounded Google/Cloudflare DNS-over-HTTPS failover and read-only error counters (TLS first byte timeout, SOCKS connection errors, DNS provider errors, fallback recoveries). It does not embed private VPS endpoints or telemetry.

For authorized LG webOS devices only, with root and Homebrew privileges. Preserve your previous package for rollback. Add test feed https://gamefree24.ru/byedpi-lg/diagnostic-r327/repository.json or sideload the IPK. **Disable ByeDPI and confirm STOPPED before upgrading** to avoid mixed old/new code. Then install the beta, Enable ByeDPI, try official YouTube 20–30 seconds, then press the in-app YouTube Check button and photograph the categorized counters. No private system logs need to be shared.

This is a **beta**: offline tests passed, but playback has NOT been verified on the neighbor's LG 65UP7600LF. DNS failover will NOT fix a blocked TLS handshake when DNS is already working. The main Homebrew feed remains unchanged.
