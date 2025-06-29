# 🛡️ Certificates Present in Xperia X1 ROM (Build PQ2)

This document catalogs the root and trusted certificates originally embedded in the system image of the Xperia X1 prototype (Build PQ2). This inventory helps assess its baseline TLS/HTTPS compatibility and identify cryptographic limitations of the original firmware.

---

## 📋 Certificate Table

| Common Name (CN)                       | Issuer                  | Expiration Date | SHA1 Fingerprint         | Notes                    |
|----------------------------------------|--------------------------|------------------|---------------------------|---------------------------|
| Example Root CA                        | Example Org              | YYYY-MM-DD       | ABCD 1234 ...             | Present in Root store     |
| Microsoft Root Certificate Authority   | Microsoft Corporation    | 2030-12-31       | 1234 5678 ...             | Used for code signing     |
| VeriSign Class 3 Primary CA            | VeriSign, Inc.           | 2028-01-07       | 89AB CDEF ...             | Detected post-reset       |

> _Note: All certificates gathered via CeRegEditor and/or screenshots of the system certificate store._

---

## 🧠 Observations

- The device contains certificates predating 2010, limiting support for TLS 1.2 and SHA-256 chains.
- Some certificates are expired but still listed as trusted in the ROM.
- Root certificates are stored under `HKLM\Security\Certificates\TrustedRoots` in the registry.

---

## 📷 Supporting Evidence

Screenshots are stored in `/device-snapshot/screenshots/`:
- `cert_panel_root_ca.jpg`
- `verisign_details.jpg`
- `timezone_default_lima.jpg` (regional context)

---

Let me know if you’d like me to add SHA-256 columns, sample registry exports, or detection tools you can run from the device. We could also cross-reference this list with modern certificate authorities to identify compatibility gaps.

