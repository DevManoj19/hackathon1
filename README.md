<h1 align="center">🛡️ GDPR-Compliant DID System for Cultural Heritage</h1>

<p align="center">
  A privacy-first Decentralized Identifier (DID) system built for managing cultural heritage data using W3C standards,<br>
  GDPR principles, and verifiable credentials. Empower museums, researchers, and artifacts with digital trust.
</p>

---

## 🧠 Project Overview

This system implements:

- ✅ DID generation using **Ed25519**
- ✅ GDPR-compliant **consent management**
- ✅ **Cultural Heritage Verifiable Credentials** issuing
- ✅ **Data Portability** (Article 20)
- ✅ **Right to be Forgotten** (Article 17)
- ✅ DID **revocation**, **audit logging**, and **Dataverse integration (mock)**

> Inspired by real-world digital preservation needs and European data rights.

---

## 📌 Features Table

| Feature | Description |
|--------|-------------|
| 🔐 DID Generation | Create W3C-compliant DIDs for artifacts, researchers, and curators |
| 🤝 Consent Recording | GDPR-aligned consent with timestamp, IP, and purpose tracking |
| 🧾 Credential Issuing | Verifiable credentials for cultural artifacts |
| 🧪 Signature System | Ed25519-based signing and signature verification |
| 🧠 Data Portability | Export all data tied to a DID (consent, audit, credentials) |
| 🗑️ Right to be Forgotten | Erase data, revoke DIDs while preserving audit logs |
| 🌐 Mock Dataverse Integration | Assign DOI, metadata, and simulate repository linking |
| 📜 Audit Logging | Every action is logged with timestamp and traceability |

---

## 🚀 Run on Google Colab

<a href="https://colab.research.google.com/github/DevManoj19/hackathon1/blob/main/hackathon_prototype.ipynb" target="_parent">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

---

## 🛠️ How to Use

1. **Clone the repo**
```bash
   git clone https://github.com/DevManoj19/hackathon1.git
   cd hackathon1
 ````

2. **Install dependencies**

   ```bash
   pip install cryptography requests
   ```

3. **Run notebook or script**

   * Open `hackathon_prototype.ipynb` in Jupyter or Google Colab.
   * Run all cells to simulate:

     * DID creation
     * Credential issuing
     * Consent logging
     * Revocation and GDPR workflows

---

## 📂 Example Outputs

* ✅ DIDs:

  * `did:heritage:<...>`
  * `did:artifact:<...>`
* 🧾 Cultural Heritage Credential:

  ```json
  {
    "@context": ["https://www.w3.org/2018/credentials/v1", ...],
    "type": ["VerifiableCredential", "CulturalHeritageCredential"],
    "issuer": "did:heritage:...",
    "credentialSubject": {
      "id": "did:artifact:...",
      "artifact": {
        "name": "Ancient Greek Amphora",
        ...
      }
    }
  }
  ```

---

## 📜 License

This project is under the **MIT License** — free to use, modify, and build upon.

---

<p align="center">
  Built with 🧠 + ❤️ with Python3 by <a href="https://github.com/DevManoj19" target="_blank">DevManoj19</a>
</p>
