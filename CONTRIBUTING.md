# Contributing to Trade Agent Skills

Thank you for helping build the world's most comprehensive open-source cross-border trade & compliance skills repository for Claude Code and AI agents!

---

## 🌟 How You Can Contribute

We actively welcome contributions across the following areas:

1. **New Country Trade Guides**:
   - Add reference templates under `skills/export-docs-generator/references/` for other major trade hubs (e.g. `japan-export-docs.md`, `vietnam-export-docs.md`, `brazil-export-docs.md`, `singapore-export-docs.md`).
2. **Customs & Tax Updates**:
   - Update GST rules, CBIC circulars, ICEGATE EDI formats, or EU/UK HMRC customs amendments.
3. **Evals & Test Cases**:
   - Add new real-world scenario prompts in `evals/eval-test-cases.json`.
4. **Integration Utilities**:
   - Add scripts/converters to export generated markdown tables to standard `.docx`, `.xlsx`, or EDIFACT/XML customs formats.

---

## 📋 Guidelines for New Skills / References

When submitting a PR for a new country or trade module:
- **Zero AI Slop**: Do not include generic placeholders like `[Insert details here]`. Use realistic, structured dummy data (e.g., realistic HS codes, real port codes, legal wording).
- **Include Boundaries**: Always clearly delineate when an AI agent must escalate to a licensed Customs Broker (CHA), Freight Forwarder, or Chartered Accountant.
- **Maintain Markdown Standard**: Ensure all tables and code fences format cleanly across terminal displays, IDEs, and GitHub markdown.

---

## 🚀 Submitting a Pull Request

1. Fork the repository.
2. Create a feature branch (`git checkout -b feature/japan-export-docs`).
3. Commit your changes with clear messages (`git commit -m "feat: add Japan export customs and invoice standard"`).
4. Push to your branch (`git push origin feature/japan-export-docs`).
5. Open a Pull Request with a summary of the regulatory basis.
