# 📱 Xperia X1 Preservation Project (Build PQ2)

This repository documents and preserves the state of a rare Xperia X1 prototype running Build PQ2. The goal is to extract, catalog, and protect system-level components, configurations, and behaviors as close as possible to their original condition.

---

## 🧭 Objective

To provide a faithful technical snapshot of the Xperia X1 (Build PQ2) — including firmware layout, hardware identifiers, system registry data, and bundled software like panels — to support digital preservation and historical study.

---

## 🧰 Environment & Tools

- Visual Studio 2008
- Windows Mobile 6 SDK
- Remote Registry access (CeRegEditor)
- ActiveSync or Windows Mobile Device Center (WMDC) for file transfers
- SharpZipLib (Remote File Viewer)
- .NET Compact Framework 3.5, 
- Git 2.10.0 for Windows XP compatibility

---

## 📂 Repository Structure

```bash
XperiaX1_Project/
├── /docs/                → Documentation in Markdown
├── /firmware/            → System dumps, ROMs, hash verification
├── /panels/              → Default and custom panels (.zip, .dll)
├── /tools/               → Utilities used during extraction
├── /certs-in-rom/        → Inventory of root certificates present in the system
├── /device-snapshot/     → Screenshots, hardware photos, metadata
└── README.md             → This document

---

## 🔐 Preservation Ethics
- All extracted content originates from a personally owned prototype.
- No commercial software or licensed ROMs are distributed.
- This repository serves educational and archival purposes only.

---

## 📸 Highlights
- Build version: `19608.1.2.60` (Windows Mobile 6.1 Professional)
- Device ID: X1a
- Processor: Qualcomm MSM7201A @ 528 MHz
- OS Language: Spanish (Latinoamérica)
- Default timezone: GMT-5 Lima/Bogotá/Quito
- Physical keyboard: English layout (missing Ñ key) key)

---

Additional screenshots and hardware photos are available in /device-snapshot/.

---

## 🧪 Areas Documented
- System registry exports and analysis
- Default panel extraction and metadata
- Trust anchor (root certificate) listing from ROM
- Hardware characteristics and configuration anomalies
- Visual state post factory reset

--- 

## 📎 Related Projects
This repository focuses exclusively on documentation and preservation. For modern enhancements (e.g. TLS updates, new browsers, messaging support), see the Xperia X1 Modernization Toolkit (coming soon).
