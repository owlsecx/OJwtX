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

OJwtX is a JWT / JWS / JWE security auditor that decodes tokens, audits claims and algorithms, compares tokens, and optionally verifies or forges HS* tokens with a supplied secret. It uses the Python standard library only (no PyJWT) and supports batch scanning, JWKS listing, and TXT/JSON/CSV export.

---

## ✨ Features

- Decode JWT header/payload/signature without verification; detect `alg`, `kid`, `typ`, and `cty`
- Security audit for `alg:none`, HS/RS confusion guidance, weak HMAC dictionary test, exp/nbf/iat skew, sensitive claims, and `kid` path hints
- Claims analyzer with iss/aud/sub/exp checklist and optional custom rules from config
- Compare two JWTs at header and claim level; batch audit from a file or Bearer extraction from logs
- JWKS fetch or offline JWKS file listing; HS* verify/forge helpers with user-supplied secret
- Export TXT / JSON / CSV; interactive menu and full CLI

---

## ⚙️ Requirements

- **Linux**
- **No Python installation needed** — runs as a standalone executable

---

## 🚀 Usage

```bash
./OJwtX --decode eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiIxIn0.sig
./OJwtX --audit TOKEN --expect-iss https://idp.example --json
./OJwtX --batch tokens.txt -o audit.csv --format csv
./OJwtX --help
```

---

## 📦 Part of OwlSec Toolkit

This tool is part of the **OwlSec** suite — a collection of 300+ security and privacy tools.

🔗 [owlsec.org](https://owlsec.org)

---

## ©️ License

MIT License — © Khaled S. Haddad

*Tools are distributed as pre-built executables. Source code is proprietary.*
