# UVRN Base

**UVRN Base** is the seed repository of the **uvrn-core** organization.  
It defines the **UVRN protocol**: schemas, receipts, and validation logic.  
This is the **genesis block** of the ecosystem. Everything else — explorers, badges, fix-it recipes — grows from here.  

---

## 🌐 What is UVRN?

UVRN is an open protocol for producing **verifiable receipts**.  
It reconciles analytics data, generates proof, and establishes trust.  

- **Checks** → structured test results (tags, events, parity, UTMs, a11y/perf)  
- **Confidence Score** → weighted score from completeness, parity, freshness  
- **Receipts** → signed, replayable records of verification runs  
- **Artifacts** → fix-it recipes (GTM JSON, CSV maps, code snippets)  

UVRN is **protocol-first**: receipts and schemas live in code, are CI-enforced, and can be replayed anywhere.  

---

## 📂 Repo Layout

```
/schemas/
  uvrn_receipt.schema.json   # canonical JSON Schema
/examples/receipts/
  hello_uvrn.json            # example receipt
/.github/workflows/
  validate-uvrn.yml          # CI validator (Ajv)
```

---

## ✅ Quickstart

Clone the repo:

```bash
git clone https://github.com/uvrn-core/uvrn-base.git
cd uvrn-base
```

Install AJV and validate example receipts:

```bash
npm install -g ajv-cli
ajv validate -s schemas/uvrn_receipt.schema.json -d "examples/receipts/*.json"
```

If everything passes, you’ll see:

```
examples/receipts/hello_uvrn.json valid
```

---

## 🛠 Roadmap

- [x] Genesis schema: `uvrn_receipt.schema.json`  
- [x] Example receipt + CI validator  
- [ ] Add `verification_run.schema.json` (multi-run structure)  
- [ ] Add `fix_recipe.schema.json` (for auto-remediation artifacts)  
- [ ] Integrate Zod + TypeScript mirroring  
- [ ] Build **Receipt Explorer UI** (in `uvrn-explorer`)  

---

## 🔑 Principles

- **Protocol-first** → schemas + receipts are canonical  
- **Replayable** → every receipt can be revalidated anywhere  
- **Proof over trust** → verification = receipts, not screenshots  
- **Extendable** → artifacts, fix-it recipes, and explorers grow from the base  

---

## 🤝 Contributing

We welcome early contributors! Start by:  

1. Reading `/schemas/uvrn_receipt.schema.json`  
2. Creating your own sample receipt under `/examples/receipts/`  
3. Submitting a pull request (CI will validate your receipt automatically)  

---

## 📜 License

Apache 2.0 — see [LICENSE](LICENSE) for details.  
