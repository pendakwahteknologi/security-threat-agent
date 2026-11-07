# Security Threat Agent

A ready-to-use guide for building an AI agent that watches public security sources and alerts you about new vulnerabilities, active exploitation, zero-days and malicious packages.

It covers 112 source links, including Malaysian sources such as MyCERT, CyberSecurity Malaysia, NACSA and NC4, plus evidence labels, alert levels and safety rules.

[Baca dalam Bahasa Melayu](#bahasa-melayu)

**The guide:** [AGENT_PROMPT.md](AGENT_PROMPT.md)

## What it does

| Area | Behaviour |
|---|---|
| Monitoring | CVEs, exploitation in the wild, zero-days, supply chain compromise, ransomware, phishing and AI or MCP vulnerabilities |
| Evidence | Separates confirmed exploitation, reported claims, scanning, public exploits and predicted risk |
| Priority | URGENT, HIGH, WATCH and DIGEST, based on your own products and exposure |
| Noise | Deduplicates reports and alerts only on new or materially changed findings |
| Safety | Treats fetched content as untrusted, never runs exploits, never scans or patches on its own |

## Quick start

1. Open [AGENT_PROMPT.md](AGENT_PROMPT.md) and copy it.
2. Fill in the `Configuration` section with your products, versions, alert destination and digest time. Anything left blank is reported as unknown exposure.
3. Give it to an AI agent that can read the web and send a message to your alert destination.
4. Ask for one run first, and check the sources and the alert format.
5. Set up a schedule so it runs on its own.

A suggested first message for the agent:

```text
Follow the instructions in AGENT_PROMPT.md. Start with the setup steps in
Source Maintenance, report which sources you can actually reach, then run one
monitoring cycle and show me the result.
```

## Before you rely on it

- **It needs a scheduler.** The prompt does nothing between runs. Automatic alerts only happen once the agent runs on a schedule or as a persistent service.
- **It does not guarantee coverage.** It can only report what is publicly disclosed and reachable. Keep your normal patching and vulnerability management.
- **Keep your filled-in configuration private.** Your asset inventory shows what an attacker would want to know. Do not post it or commit it to a public fork.
- **Some sources need more than a web fetch.** Some require accounts or API keys, and others block automated access.
- **A person should act on the alerts.** Check them against the linked primary sources before changing production systems.

## Link status

All 112 links were tested on 2026-11-07. Of these, 108 opened normally.

| Source | Result |
|---|---|
| Australian cybersecurity alerts | Timed out from the test network in Malaysia, not confirmed |
| Broadcom and VMware Support Portal | Blocked by a bot check, not confirmed |
| SentinelLABS | Blocked by a bot check, not confirmed |
| Wordfence Vulnerability Database | Returned a bot challenge, not confirmed |

These sources may need a browser, an account or another integration. Sources change over time, so run the setup steps in `Source Maintenance` before you depend on them.

## Bahasa Melayu

Panduan ini membantu anda membina ejen AI yang memantau sumber keselamatan awam dan memberi amaran tentang kelemahan baharu, eksploitasi aktif, zero-day dan pakej berniat jahat. Sumber Malaysia seperti MyCERT, CyberSecurity Malaysia, NACSA dan NC4 turut disertakan.

### Cara guna

1. Buka [AGENT_PROMPT.md](AGENT_PROMPT.md) dan salin kandungannya.
2. Isi bahagian `Configuration` dengan produk, versi, destinasi amaran dan waktu ringkasan harian anda.
3. Berikan kepada ejen AI yang boleh membaca web dan menghantar mesej ke destinasi amaran anda.
4. Jalankan sekali dahulu, kemudian semak sumber dan format amaran.
5. Tetapkan jadual supaya ejen berjalan secara automatik.

### Perkara penting

- Ejen hanya berjalan apabila dijadualkan. Prompt ini sahaja tidak akan menghantar amaran secara automatik.
- Ejen hanya melaporkan maklumat awam yang boleh dicapai, jadi teruskan proses tampalan keselamatan anda seperti biasa.
- Jangan kongsi senarai aset anda secara terbuka kerana maklumat itu berguna kepada penyerang.
- Semak amaran dengan sumber asal sebelum membuat perubahan pada sistem produksi.

## License

[CC BY 4.0](LICENSE). You may share and adapt this guide, including commercially, with credit to Pendakwah Teknologi.
