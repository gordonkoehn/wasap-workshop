# W-ASAP Workshop: Exploring SARS-CoV-2 Wastewater Data

**Hands-on workshop materials for exploring Swiss wastewater surveillance data using W-ASAP, GenSpectrum, and Loculus APIs.**

## Workshop Overview

**Duration:** 45 minutes (5 min demo + 30 min hands-on + 10 min Q&A)

**Target Audience:** Researchers who want to explore SARS-CoV-2 wastewater data themselves

**Use Cases:**
- Variant exploration
- Primer validation
- Co-occurrence analysis
- Accessing raw data programmatically

## Getting Started

### Option 1: Google Colab (Recommended)
1. Open the notebook in Google Colab: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/gordonkoehn/wasap-workshop/blob/main/wasap_workshop.ipynb)
2. Run the setup cell to import required libraries
3. Follow the exercises!

### Option 2: Local Jupyter Notebook
```bash
# Clone the repository
git clone https://github.com/gordonkoehn/wasap-workshop.git
cd wasap-workshop

# Install dependencies (optional - all are standard libraries)
pip install requests pandas matplotlib biopython

# Launch Jupyter
jupyter notebook wasap_workshop.ipynb
```

## Workshop Structure

### Section 1: GenSpectrum/Swiss-Wastewater Interface
**Browser-based exploration (no coding required)**
- Navigate the GenSpectrum interface
- Exercise 1: Find nucleotide mutations in Zürich
- Exercise 2: Track BA.3.2* variant in Basel
- Bonus: Link to clinical sequences via CovSpectrum

### Section 2: W-ASAP Loculus for Downloading Alignments
**Learn about the data backend**
- What is Loculus?
- How to download alignment data
- Where to find sequences

### Section 3: LAPIS + Loculus APIs for Programmatic Queries
**Three runnable Python code cells:**

**Cell 3a: Track Mutations Over Time**
- Query the LAPIS API for mutation frequencies
- Visualize as a heatmap
- Example: Track 3 mutations in Basel over Oct-Dec 2025

**Cell 3b: Advanced Co-occurrence Queries**
- Check if mutations occur together in samples
- Primer validation examples
- Advanced N-of-M syntax for amplicon analysis

**Cell 3c: Download Sequence Data Programmatically**
- Fetch metadata from Loculus
- Access BAM files and SILO read data
- Integrate into your research workflows

## Key Features

✅ **Live Data** - All queries use real-time APIs
✅ **Research-Ready** - Examples you can adapt for your own analysis
✅ **Educational** - Step-by-step explanations with curl examples
✅ **Error Handling** - Graceful failures with helpful messages
✅ **Reproducible** - All code is documented and ready to run

## Resources

- **GenSpectrum Interface:** [https://genspectrum.org/swiss-wastewater/covid](https://genspectrum.org/swiss-wastewater/covid)
- **Loculus Database:** [https://db.wasap.genspectrum.org/](https://db.wasap.genspectrum.org/)
- **LAPIS API Docs:** [https://lapis.wasap.genspectrum.org/swagger-ui/index.html](https://lapis.wasap.genspectrum.org/swagger-ui/index.html)
- **Loculus API Docs:** [https://api.db.wasap.genspectrum.org/backend/swagger-ui/index.html](https://api.db.wasap.genspectrum.org/backend/swagger-ui/index.html)
- **V-Pipe Scout (Advanced):** [https://wasap.genspectrum.org/](https://wasap.genspectrum.org/)
- **LAPIS Advanced Queries:** [https://lapis.cov-spectrum.org/open/v2/docs/concepts/advanced-query/](https://lapis.cov-spectrum.org/open/v2/docs/concepts/advanced-query/)

## Technical Details

**Pre-installed Libraries (Google Colab):**
- `requests` - API calls
- `pandas` - Data manipulation
- `matplotlib` - Visualization
- `json` - JSON parsing

**Optional:**
- `biopython` - Sequence parsing (install with: `pip install biopython`)

## Data Access

All data comes from the Swiss wastewater surveillance system:
- **Latest data:** Available the day after processing
- **Metadata:** Collection date, location, sequencing coverage
- **Raw alignments:** BAM files for detailed analysis
- **Read-level data:** SILO reads for variant calling

## Contributing

Found an issue or want to improve the workshop? Please open an issue or pull request!

## Citation

If you use W-ASAP data or tools in your research, please cite:
- WISE project: [https://wise.ethz.ch/](https://wise.ethz.ch/)
- GenSpectrum: [https://genspectrum.org/](https://genspectrum.org/)

## License

This workshop material is provided for educational purposes.

## Contact

For questions about the workshop or W-ASAP tools:
- Open an issue on GitHub
- Visit the WISE project website: [https://wise.ethz.ch/](https://wise.ethz.ch/)

---

**Happy exploring! 🦠💧**
