# Remote Administration Tool (RAT) - C++ [Private/Educational Use]

> ⚠️ This is a **private repository** created for **educational purposes only** in cybersecurity and systems programming.

## 🧠 Purpose

This project is a C++ implementation of a Remote Administration Tool (RAT) designed to deepen understanding of:
- Network socket programming
- Client-server architecture
- Remote command execution
- Security implications of remote access tools

## 🚨 Legal & Ethical Disclaimer

- This tool **must not** be used on any computer you do not own or do not have **explicit authorization** to access.
- The author **does not condone** illegal activity and takes no responsibility for misuse.
- This code is intended to be run in **controlled environments** such as:
  - Virtual machines
  - Cybersecurity labs
  - Educational sandboxes

## 🛠️ Features (for research/demo only)

- Command execution via remote shell
- File upload/download
- Screen capture (basic implementation)
- Keylogging (optional / toggleable)
- Encrypted client-server communication (in progress)

## 🔐 Communication Security

This RAT communicates over **HTTPS** to ensure data confidentiality and basic authentication during transmission. Key features include:

- TLS-encrypted connections using OpenSSL
- Optional client authentication (mTLS)
- Encrypted payloads in JSON or binary format
- Stealth-compatible with common web traffic patterns (for research)

> ⚠️ Certificates should be self-signed or issued by a local CA for lab testing. **Never use this over public infrastructure** without proper safeguards.

### Generating Test Certificates (OpenSSL)

```bash
openssl req -x509 -nodes -days 365 -newkey rsa:2048 \
  -keyout server.key -out server.crt

