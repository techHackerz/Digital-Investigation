# ANZ Cyber Security Management Simulation – Forage (April 2025)

This project documents my work and findings from the ANZ Australia Cyber Security Management Virtual Experience Program hosted on Forage.

## 📂 Project Overview

The simulation involved analyzing network traffic captured in a PCAP file using Wireshark and identifying potential cybersecurity threats. Tasks included extracting and analyzing images, documents, and hidden messages from HTTP traffic.

## 🛠 Tools Used

- Wireshark
- HxD Hex Editor
- Base64 Decoder
- Online ZIP Extractor

## 🧪 Key Tasks & Findings

### 🔍 Sub-task 1
- Extracted `anz-logo.jpg` and `bank-card.jpg` from PCAP by identifying HTTP GET requests and carving JPEG data based on hex signatures.

### 🔍 Sub-task 2
- Extracted `ANZ1.jpg` and `ANZ2.jpg` with hidden messages appended post image footer:
  - ANZ1: “You've found a hidden message in this file!”
  - ANZ2: “You've found the hidden message! Images are sometimes more than they appear.”

### 🔍 Sub-task 3
- Recovered a suspicious document `how-to-commit-crimes.docx` containing a message implying malicious intent.

### 🔍 Sub-task 4
- Extracted PDFs: `ANZ_Document.pdf`, `ANZ_Document2.pdf`, and `evil.pdf`.

### 🔍 Sub-task 5
- File `hiddenmessage2.txt` was a disguised JPEG image.

### 🔍 Sub-task 6
- `atm-image.jpg` contained two concatenated JPEG images in a single GET request.

###  Sub-task 7
- `broken.png` was base64 encoded. Decoded and reconstructed successfully.

###  Sub-task 8
- `securepdf.pdf` was a disguised ZIP containing an encrypted PDF. Password “secure” was found in TCP stream.

##  Artifacts

All recovered images and documents are included in this repository under the `/artifacts` directory.

##  Full Report

See [ANZ_PCAP_Investigation_Report.pdf](./ANZ_Forage_Cybersecurity/Task2/Task%202.pdf) for detailed methodology and visual evidence.

---

👤 **Author**: Akash Sebastian  
📅 **Completed**: April 2025  
