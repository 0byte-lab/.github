<p align="center">
  <img src="https://github.com/user-attachments/assets/8ffbede2-f7f3-481d-8197-7aeefbd5bd94" alt="0byte logo" width="200"/>
</p>

<h3 align="center">The trust layer for the AI internet.</h3>

<p align="center">
  0byte lets anyone cryptographically verify where AI content or actions came from.
</p>

<p align="center">
  <a href="https://github.com/0byte-lab/0byte/actions/workflows/ci.yml"><img src="https://github.com/0byte-lab/0byte/actions/workflows/ci.yml/badge.svg?branch=dev" alt="CI"></a>
  <a href="https://pypi.org/project/0byte/"><img src="https://img.shields.io/pypi/v/0byte" alt="PyPI"></a>
  <a href="https://www.npmjs.com/package/@0byte-lab/sdk"><img src="https://img.shields.io/npm/v/@0byte-lab/sdk" alt="npm"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-blue.svg" alt="License: MIT"></a>
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
  <a href="https://0byte.tech">Website</a> · <a href="https://github.com/0byte-lab/0byte">Monorepo</a> · <a href="https://x.com/0byteHQ">X</a> · <a href="https://discord.gg/2GUWSDrk">Discord</a>
</p>
