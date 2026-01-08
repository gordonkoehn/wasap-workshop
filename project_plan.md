You are helping scaffold a Google Colab notebook for a hands-on W-ASAP workshop (45 min total: 5 min demo + 30 min hands-on + 10 min Q&A).
Workshop Context:

Audience: Researchers who want to explore SARS-CoV-2 wastewater data themselves
Use cases: variant exploration, primer validation, cooccurrence analysis, accessing raw data the day after processing
Format: People work through the notebook on their laptops; you circulate answering questions
This is NOT a pitch or talk—only for people with real questions to answer


The notebook has three sections:
Section 1: GenSpectrum/Swiss-Wastewater Interface

Markdown intro: "Explore which variants are circulating"
Show how to navigate https://genspectrum.org/swiss-wastewater/covid
Primer validation example: check if N1/N2 primers cover current mutations
User explores manually in browser (no code required)

Section 2: W-ASAP Loculus for Downloading Alignments

Markdown intro: "Get your hands on real sequences"
Show https://db.wasap.genspectrum.org/
How to download alignment data
Explain: What is Loculus? Where to find sequences?

Section 3: LAPIS + Loculus APIs for Programmatic Queries
Three runnable Python code cells:
Cell 3a: LAPIS Query – Count a Set of Mutations over time 

Query: Count reads by lineage over time for Swiss wastewater
Visualize as a heatmap

Cell 3b: LAPIS Query – Primer Coverage

Query: Find reads with mutations at primer binding sites
Show: which primers are affected? What % of reads?
Practical use case: diagnose why your dPCR might be failing

Cell 3c: Loculus API Query – Metadata Inspection

Query: Fetch sample metadata from Loculus
Show: dates, locations, coverage stats


Technical:

Pre-installed: requests, pandas, matplotlib
All queries use live APIs
Simple, readable output (JSON + plots where useful)
Error handling: graceful failures with helpful messages
Comments explain what each query does + how to modify it

Tone:

Practical, not academic
"Here's how to answer your own questions"
Conversational comments, not formal

Do NOT include:

RSV-A, Influenza (not live yet—comment out for future)
Complex statistical analysis (keep it exploratory)
Long explanations (let the code speak)

Please scaffold this notebook. I'll iterate and refine it with you.