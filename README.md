# var2lit
Variant-to-literature batch tool for retrieving bibliographic metadata (titles, abstracts, PMIDs, etc.) using LitVar and NCBI APIs, based on genetic variant identifiers (e.g., rsIDs, HGVS).

---

## Overview

`var2lit` streamlines the process of retrieving literature metadata for genetic variants by automating batch queries using the **LitVar API** and **NCBI Entrez API**.  
It helps users bypass the one-by-one search limitations of the LitVar website and enables faster access to variant-linked article titles, abstracts, publication dates, and PMIDs.

This tool is particularly useful for:
- Researchers performing variant annotation
- Genomics analysts working on literature curation
- Anyone needing to programmatically link variants to scientific publications

---

## Key Features

- **Batch input** of multiple variant identifiers (rsIDs, HGVS)
- **Retrieves** titles, abstracts, PMIDs, publication dates
- **Outputs** structured results (e.g., CSV)
- Built with Python and designed to run in Jupyter or CLI
- Extensible for downstream NLP, annotation, or visualization

---

## Example Input

A simple list of variant identifiers:
rs781394307
rs766444643


---

## Example Output

| Variant ID | PMID | Title | Abstract | Publication Date |
|------------|------|-------|----------|------------------|
| rs781394307 | 33546694 | BMC biology | Abstract content here... | 2021 |
| rs766444643 | 33546694 | BMC biology | Abstract content here... | 2021 |

---

## Usage

Coming soon — full step-by-step instructions for:

- Setting up environment
- Running the pipeline
- Understanding output formats

---

## Dependencies

- Python 3.10+
- `requests`
- `pandas`
- `biopython` *(if using Entrez queries)*
- `tqdm` *(optional, for progress bars)*

> You can install dependencies using:  
> `pip install -r requirements.txt` *(to be added)*

---

## License

This project is licensed under the **GNU General Public License v3.0**.  
You are free to use, modify, and distribute this work, but any redistributed versions must also be open-source under the same license. See `LICENSE` for full details.

---

## Acknowledgements

- Variant data queried through [LitVar](https://www.ncbi.nlm.nih.gov/research/litvar/)  
- Article metadata retrieved via [NCBI Entrez](https://www.ncbi.nlm.nih.gov/books/NBK25499/)

---

## Future Plans

- Add automated summarization of abstracts (using Hugging Face)
- Create a web-based or command-line interface
- Allow optional filtering by journal

---

## Author

Cristina Delgado  
Emerging Leaders in Data Science Fellow, NIAID/NIH

---

