# JWT Fundamentals

A complete reference on JSON Web Tokens: what they are, how to create and validate them, the cryptographic algorithms behind JSON Web Signatures (JWS) and JSON Web Encryption (JWE), and security best practices for JWT-based systems.

All five modules are consolidated into a single Jupyter Notebook: [`jwt-fundamentals.ipynb`](jwt-fundamentals.ipynb).

## Modules

| # | Title | Topics |
|---|---|---|
| 01 | Why JWTs? | JWT structure, OAuth 2, OpenID Connect, the JOSE standards family, when to (and not to) use JWTs |
| 02 | Using JSON Web Tokens | Token creation, base64url encoding, claims validation, standard claim types, RFC 9068 access tokens |
| 03 | JSON Web Signatures (JWS) in Depth | Digital signatures, RSASSA-PKCS1-v1_5, RSASSA-PSS, ECDSA, EdDSA, HMAC — algorithm selection |
| 04 | JSON Web Encryption (JWE) in Depth | Hybrid encryption, JWE token structure, key-encryption algorithms, content-encryption algorithms, nested JWTs |
| 05 | JWT Security Best Practices | Cryptographic agility attacks, embedded key attacks, claims enforcement, revocation, mTLS, DPoP, PASETO, BFF pattern |

## Usage

Open the notebook in Jupyter or any compatible environment:

```bash
jupyter notebook jwt-fundamentals.ipynb
```

Diagram images are embedded via `assets/` relative paths — keep the `assets/` directory alongside the notebook.

## Assets

The [`assets/`](assets/) directory contains 14 educational diagrams extracted and cleaned from the course slide decks:

| File | Description |
|---|---|
| `01-jwt-issuer-recipient-flow.png` | Issuer → HTTP request → Recipient with token |
| `02-oauth-players.png` | The four OAuth 2 players |
| `03-oauth-dance.png` | OAuth 2 authorization code flow |
| `04-token-validation-token-store.png` | Stateful token lookup via token store |
| `05-token-validation-stateless.png` | Stateless JWT validation |
| `07-digital-signatures.png` | Digital signature: Alice (private key) → Bob (public key) |
| `08-openid-connect-dance.png` | OpenID Connect flow with identity provider |
| `10-digital-signatures-attack.png` | One signer, multiple independent verifiers |
| `11-hmac-token-issuer-recipient.png` | HMAC symmetric flow |
| `12-asymmetric-encryption.png` | Asymmetric encryption: encrypt with public key, decrypt with private |
| `13-hybrid-encryption-encrypt.png` | Hybrid encryption — sender side |
| `14-hybrid-encryption-decrypt.png` | Hybrid encryption — recipient side |
| `15-token-blocklist-flow.png` | Token blocklist revocation flow |
| `16-mtls-flow.png` | Full OAuth dance with mTLS client authentication |
