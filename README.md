# W-ASAP Workshop: Exploring SARS-CoV-2 Wastewater Data

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gordonkoehn/wasap-workshop/blob/main/wasap_workshop.ipynb)

> **Hands-on workshop materials for exploring Swiss wastewater surveillance data**

---

## 📋 About

**Author:** Gordon J. Koehn
**Event:** WISE Symposium, D-BSSE / ETH Zürich
**Date:** January 16, 2026

**Duration:** 45 minutes
**Format:** 5 min demo + 30 min hands-on + 10 min Q&A

**Target Audience:** Researchers who want to explore SARS-CoV-2 wastewater data programmatically

---

## 🚀 Quick Start

Click the badge above to open in Google Colab, or clone locally:

```bash
git clone https://github.com/gordonkoehn/wasap-workshop.git
cd wasap-workshop
jupyter notebook wasap_workshop.ipynb
```

---

## 📚 What You'll Learn

### 🔍 Section 1: GenSpectrum Interface
**Browser-based exploration** (no coding required)
- Navigate the GenSpectrum interface
- Find nucleotide mutations in Zürich
- Track BA.3.2* variant in Basel
- Link to clinical sequences via CovSpectrum

### 📦 Section 2: Loculus Database
**Understanding the data backend**
- What is Loculus?
- How to download alignments
- Where to find sequences

### 💻 Section 3: Programmatic Queries
**Three runnable Python code cells:**

**Cell 3a:** Track mutations over time with LAPIS API
**Cell 3b:** Advanced co-occurrence & primer validation
**Cell 3c:** Download sequence data programmatically

---

## ✨ Key Features

- 🔴 **Live Data** — Real-time API queries
- 🔬 **Research-Ready** — Adapt examples for your analysis
- 📖 **Educational** — Step-by-step with curl examples
- 🛡️ **Robust** — Error handling with helpful messages
- 📝 **Reproducible** — Fully documented code

---

## 🔗 Resources

### Data & APIs
- [GenSpectrum Interface](https://genspectrum.org/swiss-wastewater/covid)
- [Loculus Database](https://db.wasap.genspectrum.org/)
- [LAPIS API Docs](https://lapis.wasap.genspectrum.org/swagger-ui/index.html)
- [Loculus API Docs](https://api.db.wasap.genspectrum.org/backend/swagger-ui/index.html)

### Advanced Tools
- [V-Pipe Scout](https://wasap.genspectrum.org/)
- [LAPIS Advanced Queries](https://lapis.cov-spectrum.org/open/v2/docs/concepts/advanced-query/)

### Project
- [WISE Project](https://wise.ethz.ch/)
- [GenSpectrum](https://genspectrum.org/)

---

## 🦠 Data Access

All data from the Swiss wastewater surveillance system:
- Latest data available the day after processing
- Metadata: collection date, location, sequencing coverage
- Raw alignments: BAM files for detailed analysis
- Read-level data: SILO reads for variant calling

---

## 📄 Citation

If you use W-ASAP data or tools in your research, please cite:
- **WISE project:** [wise.ethz.ch](https://wise.ethz.ch/)
- **GenSpectrum:** [genspectrum.org](https://genspectrum.org/)

---

## 📬 Contact

Questions about the workshop or W-ASAP tools?
- Open an issue on GitHub
- Visit [wise.ethz.ch](https://wise.ethz.ch/)

---

**Happy exploring! 🦠💧**
