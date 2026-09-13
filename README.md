# Silicoin: A Two-Asset, Isolated Multi-Layer Settlement Network

Silicoin is a native dual-token economy designed to resolve the single-token dilemma by separating wealth preservation from transactional utility. 

By comprising Gold (a store of value with a tail emission) and Cash (a medium of exchange balanced by market dynamics), the protocol maintains internal economic equilibrium without relying on external pegs, vulnerable third-party oracles, or gameable algorithmic loops. Furthermore, Silicoin scales horizontally via Layer Development Kits (LDKs) and is secured from genesis using ML-DSA-65 post-quantum cryptography.

Authored by Jonathan Miller (`silicoindev@proton.me`).

---

## Repository Contents

*   **`WHITEPAPER.pdf`**: The official Silicoin protocol specification.
*   **`jonathan_miller_pub.asc`**: The author's PGP public key.
*   **`WHITEPAPER.pdf.asc`**: The detached PGP signature used to cryptographically prove the authenticity and integrity of the PDF.

---

## Cryptographic Verification

To ensure the whitepaper has not been tampered with and was officially signed by the author, you can verify the detached PGP signature locally[cite: 3]. 

**1. Download the files**
Ensure `WHITEPAPER.pdf`, `WHITEPAPER.pdf.asc`, and `jonathan_miller_pub.asc` are all downloaded into the same directory.

**2. Import the public key**
```bash
gpg --import jonathan_miller_pub.asc
```

**3. Verify the signature

Bash
gpg --verify WHITEPAPER_2.pdf.asc WHITEPAPER_2.pdf
Expected Output:
If the file is pristine, your terminal will output:
Good signature from "Jonathan Miller <silicoindev@proton.me>"

If the document has been altered in any way, the system will return a BAD signature warning.
