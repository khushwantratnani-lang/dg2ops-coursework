# Threat model
| Threat | Asset | Attack | Control | Residual risk |
|---|---|---|---|---|
| Unauthenticated client | Allocation logic | Connects and sends requests | TLS + token + client ID checked before requestResources() | |
| Malformed request | Server | Bad/oversized input | Input validation, safe errors | |
| Forged ticket | Gate entry | Fake ticket | Ed25519 signature | |
| Screenshot ticket | Gate entry | Reused QR | TOTP | |
| Double entry | Gate entry | Same ticket at 2 gates | HMAC-synced entry lists + hub alert | |
