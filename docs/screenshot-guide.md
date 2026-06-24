# Screenshot and Image Guide

The uploaded documents contain useful screenshots, but several are not safe to publish as-is. Use images only after redaction or recreate them as clean diagrams.

## Recommended Screenshot Locations

| Image File | Folder | Use In | What To Show |
|---|---|---|---|
| `01-tls-certificate-chain.png` | `assets/screenshots/` | `docs/pki-tls-analysis.md` | Cropped certificate hierarchy only. |
| `02-tls-record-types.png` | `assets/screenshots/` | `docs/pki-tls-analysis.md` | Cropped TLS record type fields only. |
| `03-traceroute-sanitized.png` | `assets/screenshots/` | `docs/network-protocol-analysis.md` | Sanitized route diagram with IPs removed. |
| `04-service-discovery-sanitized.png` | `assets/screenshots/` | `docs/network-protocol-analysis.md` | Sanitized service table with hostnames/IPs removed. |
| `05-ipsec-anti-replay.png` | `assets/screenshots/` | `docs/ipsec-wireless-security.md` | Self-created diagram of sequence numbers and anti-replay window. |
| `06-ecb-cbc-comparison.png` | `assets/screenshots/` | `docs/cryptography-foundations.md` | Self-created visual comparing ECB pattern leakage vs CBC pattern hiding. |

## Images From Uploaded Documents

| Source Image Type | Publish? | Reason |
|---|---|---|
| Encrypted email screenshot | No | Shows student email/UIN and academic communication metadata. |
| Route terminal screenshot | Not raw | Shows terminal prompt and real/private network details; recreate as a sanitized diagram. |
| Registry lookup screenshots | Not raw | Can expose contact details and raw query output; summarize instead. |
| Service-discovery screenshot | Not raw | Shows host/service details and lab network artifacts. |
| Certificate viewer screenshot | Maybe, after crop | Safe only if cropped to certificate hierarchy and no personal/course details are visible. |
| TLS field screenshot | Maybe, after crop | Safe only if cropped to protocol field names and no local/session details are visible. |
| Home Wi-Fi screenshot | No | May expose SSID, device, network, or location metadata. |

## Best Practice

For this repo, prefer Mermaid diagrams, SVG diagrams in `assets/diagrams/`, cropped certificate/TLS field screenshots after redaction, and sanitized tables instead of raw terminal screenshots.

## Markdown Examples

From a file inside `docs/`:

```md
![TLS certificate chain](../assets/screenshots/01-tls-certificate-chain.png)
```

From the root README:

```md
![Protocol map](assets/diagrams/crypto-protocol-map.svg)
```

## Redaction Checklist Before Uploading Any Image

- Remove student ID, UIN, email, and course details.
- Remove VM usernames and terminal prompts.
- Remove real IP addresses, subnets, SSIDs, MAC addresses, and device names.
- Remove packet payloads, session randoms, full public-key blocks, and long modulus values.
- Crop tightly so only the concept or field being explained remains.
