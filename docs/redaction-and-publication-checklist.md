# Redaction and Publication Checklist

Use this checklist before publishing screenshots, PDFs, DOCX exports, packet captures, or generated images to this repository.

## Do Not Publish

| Item | Why It Should Not Be Public |
|---|---|
| Raw homework PDFs/DOCX files | They may include course metadata, student identifiers, professor details, and raw answers. |
| Raw resume file | It contains personal contact information and should not be inside a public project repository. |
| Full terminal screenshots | They may show VM usernames, prompts, real IPs, and lab network details. |
| Packet captures | They may expose local IPs, session metadata, DNS queries, or application traffic. |
| Public-key blocks and fingerprints | Long key material distracts from the portfolio and can create unnecessary exposure. |
| Encrypted/decrypted challenge strings | They make the repo look like answer dumping rather than professional analysis. |
| Home Wi-Fi screenshots | They may expose SSID, device, MAC address, IP address, or location context. |
| Full certificate modulus/serial screenshots | Summarize the concept instead of publishing long identifiers. |
| Raw scans or service lists | Keep hostnames, IPs, and lab targets private. |

## Safe to Publish

| Safer Artifact | Condition |
|---|---|
| Concept summaries | Explain the security principle without dumping raw answers. |
| Sanitized protocol diagrams | Use Mermaid or SVG diagrams you created yourself. |
| Certificate-chain summary | Use a small diagram or cropped hierarchy only. |
| TLS record-type table | Keep it generic and avoid packet payloads or local/session values. |
| Sanitized route diagram | Replace real hops with generic labels like Local Gateway, Upstream Network, Destination. |
| Defensive control tables | Focus on mitigations and secure design principles. |

## Public Disclaimer to Keep

Use this language in the README and any LinkedIn/GitHub description:

> This is a sanitized academic/portfolio case study. It does not contain private keys, credentials, student identifiers, raw packet captures, internal network data, home Wi-Fi screenshots, or unredacted coursework pages.

## Final Pre-Publish Review

Before pushing any new file:

- [ ] No UIN, student ID, phone number, email, or professor name.
- [ ] No raw assignment cover page or answer sheet.
- [ ] No raw packet captures.
- [ ] No VM usernames, terminal prompts, real IP addresses, or subnets.
- [ ] No SSIDs, MAC addresses, home network details, or device names.
- [ ] No long public-key blocks, certificate modulus values, or session randoms.
- [ ] No screenshots showing course submission or email metadata.
- [ ] File adds evidence of skill: protocol reasoning, cryptography, PKI, TLS, IPSec, network security, or documentation.

## Good GitHub Hygiene

- Use sanitized Markdown artifacts instead of raw documents.
- Use self-created diagrams where possible.
- Keep screenshots tightly cropped and redacted.
- Avoid making the repo look like homework answers.
- Prefer concise technical explanations and evidence maps.
