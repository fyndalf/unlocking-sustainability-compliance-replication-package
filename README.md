# Replication Package for *Unlocking Sustainability Compliance: Characterizing the EU Taxonomy for Business Process Management*

This provides a replication package for our study on characterizing the EU taxonomy for sustainable activities regarding its potential to be used for compliance monitoring with conformance checking.

Be advised that the prompt template and raw results speaks of control flow constraints "within" and "between" activities, while we in fact mean activity existence constraints and "traditional "control flow constraints. We found that this produced more plausible results, perhaps due to the symmetry with other constraints that can in fact be "within" and "between" activities

## Requirements

- Python 3.10 and pip3
- A free account with [Groq](https://groq.com/)
- A stable (!) internet connection

## Instructions

- Create an API key at [https://groq.com](https://groq.com/) and put it into the `.env` file at the top level of this repository
- Install all needed dependencies with `pip3 install -r requirements.txt`
- For getting the most recent version of the taxonomy, download it from [here](https://ec.europa.eu/sustainable-finance-taxonomy/assets/documents/taxonomy.xlsx) and put it into the `taxonomy` folder. We also provide a version from June 20 2024
- Execute the jupyter notebook `classification/constraint_extraction.ipynb` step by step, from top to bottom
- Then, run the `figures/visualizations.ipynb` for creating the according figures

## Sources

All data and taxonomy excerpts provided herein were taken from the following sources:

<https://ec.europa.eu/sustainable-finance-taxonomy/assets/documents/CCM%20Appendix%20A.pdf>
<https://ec.europa.eu/sustainable-finance-taxonomy/assets/documents/CCM%20Appendix%20B.pdf>
<https://ec.europa.eu/sustainable-finance-taxonomy/assets/documents/CCM%20Appendix%20C.pdf>
<https://ec.europa.eu/sustainable-finance-taxonomy/assets/documents/CCM%20Appendix%20D.pdf>
<https://ec.europa.eu/sustainable-finance-taxonomy/assets/documents/CCM%20Appendix%20E.pdf>
<https://ec.europa.eu/sustainable-finance-taxonomy/assets/documents/taxonomy.xlsx>

For generating the prompt template and the pipeline, we adhered to the following guidance:

<https://github.com/meta-llama/llama-recipes/blob/main/recipes/quickstart/Prompt_Engineering_with_Llama_3.ipynb>
<https://community.openai.com/t/cheat-sheet-mastering-temperature-and-top-p-in-chatgpt-api/172683>
<https://console.groq.com/playground>
