# Security and privacy / Безопасность и приватность

## Public 0.6.32

- No bundled user credentials, SSH private keys, per-device IDs or secrets.
- No bundled private VPS addresses in the DNS/SNI bridge.
- No GameFree24 telemetry client or automatic off-device diagnostics.
- Strictly local status logs; do not share them without manual redaction.
- The service requires root/Homebrew permissions on supported TV firmware; this is an important trust boundary.
- The IPK has inspectable JavaScript and shell code; binary distribution does **not** make it secret.
- This beta has passed static package and isolated DNS mounting regression tests. It has **not** passed physical post-install LG tests.

## Reporting problems / Сообщение об ошибках

Provide TV model, webOS version, app build, symptoms, and sanitized logs. Never post credentials, serial numbers, household IPs, private keys or unredacted complete logs. Do not test or alter TVs that you do not own or administer.

Always keep a working rollback package. The installer has no boot-time root hook; do not assume automatic activation after reboot.