# Key-Audit-Chain

A **Resilient and Reliable Key Management Framework** for DID-Based Decentralized Environments.


✨ Overview

**Key-Audit-Chain (KAC)** is an integrated authentication framework designed to enhance trust, key security, and auditability in Self-Sovereign Identity (SSI) environments.  
It addresses critical challenges such as:
- Real-time verification of Verifiable Credentials (VCs)
- Threshold signature-based key management (using FROST)
- Trusted Third Party (TTP)-based auditing
- Multi-VC validation for complex scenarios

📌 Features

- 🔐 **Threshold Signature:** Secure key generation & signing with the FROST algorithm.
- 📑 **Multi-VC Validation:** Pre-verify multiple credentials before Verifiable Presentation (VP) generation.
- 🔍 **Metadata Audit:** Track signature hashes & cluster IDs for anomaly detection.
- 🤝 **Interoperability:** WACI-based protocol compliance for compatibility with diverse SSI ecosystems.
- 🔄 **Key Lifecycle Management:** Support for key revocation, recovery, and real-time status checks.



## ⚙️ Installation

> **Prerequisites:**  
> - Python 3.9+
> - `pip` (Python package manager)
> - `git` installed and configured

1. **Clone the Repository**
   ```bash
   git clone https://github.com/DolJihwan/Key-Audit-Chain.git
   cd Key-Audit-Chain

2. Set up a virtual environment (optional but recommended)
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows

3. Install dependencies
   pip install -r requirements.txt


📂 Project Structure

Key-Audit-Chain/
 ├── BACKUP/             # Backup key shares and recovery logic
 ├── issuer_01/          # Issuer Node 1 (VC issuer)
 ├── issuer_02/          # Issuer Node 2 (VC issuer)
 ├── rp/                 # Relying Party modules for VC/VP validation
 ├── TTP/                # Trusted Third Party audit and verification
 ├── WALLET/             # User wallet for credential management
 ├── README.md           # Project description
 ├── requirements.txt    # Python dependencies
 └── manage.py           # Entry point for running the framework


🛡️ Security Considerations
Uses FROST for round-optimized Schnorr threshold signatures.
All signature and key management metadata is logged via a TTP.
Supports risk scoring and anomaly detection for identity spoofing prevention.


📄 License
This project is licensed under the MIT License. See LICENSE for details.


✏️ Authors
Jihwan Kim — Seoul National University of Science and Technology
Younho Lee — Professor, SeoulTech
Dae-seon Choi — Professor, Soongsil University
 

📬 Contact & Info  
For any inquiries related to this project, please contact Jihwan Kim at jihwan0724@gmail.com.  
The related research paper describing this system is currently *in submission*.
