# 🦉 OJwtX

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Linux-0a0c10?style=flat-square"/>
  <img src="https://img.shields.io/badge/Category-OWeb-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/License-MIT-green?style=flat-square"/>
  <img src="https://img.shields.io/badge/Part%20of-OwlSec%20Toolkit-7b5ea7?style=flat-square"/>
  <img src="https://img.shields.io/badge/Version-1.0.0-cyan?style=flat-square"/>
</p>

> **OJwtX** — JWT / JWS / JWE Security Auditor

---

> ⚠️ **AUTHORISED USE ONLY** — Use only on systems you own or have explicit written permission to test. Unauthorised use is illegal.

---

## 📌 Overview

JWT / JWS / JWE security auditor & lab forge helpers

---

## ✨ Features

- Decode JWT header/payload/signature without verify; pretty-print claims; detect alg, kid, typ, cty
- Security auditor — alg:none, HS/RS confusion guidance, weak HMAC dictionary (~200 secrets) offline test, exp/nbf/iat skew, missing exp, oversized tokens, sensitive claims, kid path traversal / JWKS URL hints
- Claims analyzer — iss/aud/sub/exp checklist + custom claim rules from ~/OJwtX/config.json
- Compare two JWTs (header + claim-level diff)
- Lab-only forge helpers — rebuild HS* tokens with a user-supplied secret/key file (ethical-use banner)
- JWKS fetch (urllib + timeout) and offline JWKS file
- Batch scan (one token per line) + Bearer extraction from HTTP logs / HAR-like text
- Export TXT / JSON / CSV; save chooser ~/OJwtX; clipboard
- Full CLI (--decode, --audit, --batch, --secret, --jwks)
- Interactive menu + settings persistence

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OJwtX
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
