# Contributing to UVRN Base

🎉 First off, thank you for considering contributing to **UVRN Base**!  
This project defines the **UVRN protocol** — schemas, receipts, and validation logic.  
Contributions help evolve UVRN into a stronger, more trusted standard.  

---

## 🚀 How to Contribute

We welcome contributions in the following areas:

- **Schemas** → propose or refine JSON Schemas in `/schemas/`
- **Receipts** → add example receipts to `/examples/receipts/`
- **Validation** → improve validation workflows, tests, or CI configs
- **Docs** → improve this README, CONTRIBUTING guide, or inline schema documentation

---

## 📂 Repo Structure

```
/schemas/               # Protocol schemas (JSON Schema)
/examples/receipts/     # Example receipts (JSON)
/.github/workflows/     # CI validation and linting
```

---

## 🛠 Development Workflow

1. **Fork the repository**  
   Click "Fork" at the top right of this repo.

2. **Clone your fork**  
   ```bash
   git clone https://github.com/<your-username>/uvrn-base.git
   cd uvrn-base
   ```

3. **Install dependencies**  
   AJV is used for schema validation.  
   ```bash
   npm install -g ajv-cli
   ```

4. **Make your changes**  
   - Add or edit schemas in `/schemas/`  
   - Add or update example receipts in `/examples/receipts/`  
   - Ensure your receipts validate against the schema

5. **Validate your changes**  
   ```bash
   ajv validate -s schemas/uvrn_receipt.schema.json -d "examples/receipts/*.json"
   ```

6. **Commit and push**  
   ```bash
   git checkout -b feature/my-change
   git commit -am "Add new schema/receipt example"
   git push origin feature/my-change
   ```

7. **Submit a Pull Request**  
   Open a PR against `main` in **uvrn-core/uvrn-base**.

---

## ✅ Contribution Guidelines

- Keep schemas **backward-compatible** where possible.  
- Use **clear, descriptive commit messages**.  
- Ensure all **CI checks pass** before submitting a PR.  
- Discuss major changes in an **issue** before opening a PR.  

---

## 🧩 Roadmap for Contributors

- Add more schema types (`verification_run.schema.json`, `fix_recipe.schema.json`)  
- Expand example receipts (`happy_path.json`, `parity_warn.json`, `freshness_fail.json`)  
- Improve CI validation and test coverage  
- Contribute documentation, diagrams, or explorer UI concepts  

---

## 📜 License

By contributing, you agree that your contributions will be licensed under the [MIT License](LICENSE).  
