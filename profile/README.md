<p align="center">
  <img src="https://github.com/user-attachments/assets/8ffbede2-f7f3-481d-8197-7aeefbd5bd94" alt="0byte logo" width="200"/>
</p>

<h3 align="center">The trust layer for the AI internet.</h3>

<p align="center">
  0byte lets anyone cryptographically verify where AI content or actions came from.
</p>

<p align="center">
  <a href="https://0byte.tech">
    <img src="https://img.shields.io/badge/Website-0byte.tech-1abc9c?style=for-the-badge" alt="Website">
  </a>
  <a href="https://pypi.org/project/0byte">
    <img src="https://img.shields.io/badge/PyPI-0byte-blue?style=for-the-badge" alt="PyPI">
  </a>
  <a href="https://www.npmjs.com/package/@0byte-lab/sdk">
    <img src="https://img.shields.io/badge/npm-@0byte--lab/sdk-red?style=for-the-badge" alt="npm">
  </a>
  <a href="https://x.com/0byteHQ">
    <img src="https://img.shields.io/badge/X-@0byteHQ-black?style=for-the-badge" alt="X">
  </a>
  <a href="https://discord.gg/2GUWSDrk">
    <img src="https://img.shields.io/badge/Discord-Join-5865F2?style=for-the-badge" alt="Discord">
  </a>
</p>

---

Every piece of AI-generated content — images, video, audio — gets a **cryptographic proof of origin**: what model created it, when, and by whom.

Think SSL certificates, but for AI content.

### How it works

1. **Stamp** — AI content is perceptually fingerprinted and signed with Ed25519. The proof is anchored in a Merkle transparency log.
2. **Verify** — Anyone can verify content against the registry. Perceptual hashing means verification survives screenshots, compression, and re-encoding.
3. **Trust** — Every proof is independently verifiable, tamper-evident, and publicly auditable.

### Get started

```bash
pip install 0byte          # Python
npm install @0byte-lab/sdk # TypeScript
```

```python
from zerobyte import Client

client = Client(api_key="0b_key_...")
proof = client.stamp(content, "image/png", "openai", "dall-e-3")
```

### Built with

Rust · Ed25519 · Merkle Trees · Perceptual Hashing · Multi-Index Hashing

<p align="center">
  <a href="https://github.com/0byte-lab/0byte">View the monorepo →</a>
</p>
