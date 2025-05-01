# 📄 Kapodistrian Scientific Document Signing System

This repository provides public verification tools and guidance for validating the authenticity of scientific documents officially signed by the **Kapodistrian Academy of Science (KAS)**.

All official `.pdf` documents bearing the `SIGNED_KAS` stamp are:
- Authored by verified researchers
- Integrity-protected using SHA-256 cryptographic fingerprints
- Signed by the Academy’s private key
- Accompanied by `.sha256` and `.sig` companion files

---

## 📝 Submit Your Paper for Signing

To have your finalized scientific document cryptographically signed by the Kapodistrian Academy of Science, use the official submission form:

🔗 [Submit your paper here](https://forms.gle/oLhKr2KA17NPhSvr9)

KAS will:
- Stamp your PDF with metadata and cryptographic fingerprint
- Generate and sign the official `.sha256` hash
- Return a verified bundle (.pdf, .sha256, .sig) for publication or public release

---

## 🔍 What You Can Do Here

### ✅ 1. Verify Official Document Authenticity

Use the included notebook to:
- Upload the `.pdf`, `.sha256`, and `.sig` files
- Confirm that the document matches its signed fingerprint
- Ensure the signature was issued by the **Academy’s public key**

---

## 📄 Official File Naming Convention

All official documents follow this format:

```
[AuthorLastName]_[ShortTitle]_v[Version]_SIGNED_KAS_[Date].pdf
```

Example:
```
Valamontes_SpectralRealization_v1_SIGNED_KAS_2025-05-01.pdf
```

Each document is accompanied by:
- `[...].sha256` — file hash
- `[...].sha256.sig` — cryptographic signature

---

## 🛡 Signature Verification Tools

### [`KAS_Verifier_OpenSSL.ipynb`](./KAS_Verifier_OpenSSL.ipynb)

- Upload `.sha256`, `.sig`, and `public_key.pem`
- Automatically confirm whether the signature is valid
- Verifies that the file was signed by KAS and has not been tampered with

---

## 🚀 Open Verifier Notebook

Use the official KAS OpenSSL Verifier in Google Colab to validate signed documents:

[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Galactic-Code-Developers/kas-pdf-auth-verifier/blob/main/KAS_Verifier_OpenSSL.ipynb)

📄 [Download Notebook](https://github.com/Galactic-Code-Developers/kas-pdf-auth-verifier/raw/main/KAS_Verifier_OpenSSL.ipynb)  
🔐 [Download public_key.pem](https://github.com/Galactic-Code-Developers/kas-pdf-auth-verifier/raw/main/public_key.pem)

---

## 📥 Official Public Key

The `public_key.pem` provided in this repository is the only accepted key for verifying KAS-signed documents.

Do not trust any `.sig` unless it validates with this key.

---

## ⚠️ Important Trust Policy

- Only the **Kapodistrian Academy of Science** is authorized to issue `.sig` files.
- This repository does **not** include signing tools, private keys, or signing access.
- Public users may verify signatures, but may **not generate their own**.
- Documents without a matching `.sig` file and public key validation are considered **unauthenticated**.

---

## 🔒 Trust & Transparency

Official KAS-signed documents may optionally include:
- A TRIM-CERT evaluation certificate (scientific trustworthiness)
- DOI and author metadata
- Institutional footer from the Kapodistrian Academy of Science

---

## License

This repository and all included software tools are provided under the MIT License.

All document signatures, intellectual property verifications, and validation policies are governed by the **Kapodistrian Academy of Science**.
---

## ⚖️ Disclaimer & Terms of Use

The Kapodistrian Academy of Science (KAS) provides this digital verification and signature framework as a **free academic trust service** for authors, reviewers, and institutions.

### By using this service, you acknowledge and agree that:

- All submitted documents must be final and unaltered post-submission.
- Cryptographic signatures issued by KAS confirm:
  - The document was received from the declared author
  - It passed institutional review for integrity and authorship metadata
- Use of this service is limited to academic validation, research authentication, and author attribution.
- The **primary author’s name and email** must match the metadata submitted. Any mismatch will result in rejection or revocation of the signed document.
- KAS assumes no responsibility for misuse or unauthorized redistribution of signed files.

For official verification, inquiries, or institutional adoption, contact: `security@kapodistrian.edu.gr`
