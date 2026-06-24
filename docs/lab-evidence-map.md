# Lab Evidence Map

This file maps the source work to public-safe portfolio evidence. It helps the repository show skill without uploading raw homework files.

## Evidence Mapping

| Source Area | Public Artifact | What To Show Publicly | What To Keep Private |
|---|---|---|---|
| Cryptography assignment | `cryptography-foundations.md` | Concept summaries for encoding, ciphers, RSA, PGP, MACs, and signatures | Raw decrypted challenge strings, fingerprints, public-key blocks, assignment answers |
| Certificate analysis | `pki-tls-analysis.md` | Certificate chain model, CA trust explanation, CRL concept, signature algorithm summary | Full browser screenshots, long modulus values, certificate serial screenshots |
| TLS / Wireshark work | `pki-tls-analysis.md` | TLS content types, cipher-suite explanation, Client Hello / Server Hello flow | Raw packet captures, session random values, full Wireshark window screenshots |
| Network diagnostics | `network-protocol-analysis.md` | Traceroute interpretation, filtered-hop explanation, scanning hygiene | Raw IPs, VM usernames, university network details, terminal prompts |
| Service discovery | `network-protocol-analysis.md` | General service-exposure reasoning and defensive monitoring ideas | Full scan output, real host lists, exact lab subnets |
| IPSec | `ipsec-wireless-security.md` | Anti-replay windows, Security Associations, network-layer transparency | Raw diagrams from assignment pages if they contain course metadata |
| Wireless security | `ipsec-wireless-security.md` | WEP weakness summary and WPA2/WPA3 migration logic | Home Wi-Fi SSID, MAC address, IP address, device names, location metadata |

## Suggested Public Evidence Strength

| Evidence Type | Strength | Notes |
|---|---|---|
| Original diagrams created in Markdown/Mermaid | High | Best public-safe visual evidence. |
| Sanitized certificate-chain screenshot | Medium | Safe only if cropped and no personal/course data is visible. |
| Sanitized Wireshark TLS field screenshot | Medium | Crop to field names; avoid packet payloads or local IP details. |
| Raw assignment screenshot | Low | Avoid. Often includes course, personal, or raw lab details. |
| Full PDF upload | Very low | Do not publish. It looks like schoolwork and may expose identifiers. |

## Recruiter Framing

A strong explanation is:

> I reviewed crypto and network security lab work, extracted the reusable security lessons, and converted them into public-safe documentation. The repo focuses on protocol reasoning, certificate trust, TLS behavior, IPSec protections, and network-security interpretation rather than raw assignment answers.
