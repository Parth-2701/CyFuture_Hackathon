# CyFuture_Hackathon
This repository contains the data and code files required for building a Legal Contract Reviewer for english contracts using the CUAD dataset.

## Dataset Used

This project leverages a subset of the **Contract Understanding Atticus Dataset (CUAD)** to automate legal contract analysis. CUAD is an expert-annotated dataset designed for **high-precision clause extraction**, featuring:

- **500+ contracts**
- **13,000+ labeled clauses**
- **41 specialized legal categories**

By utilizing CUAD, this system enhances efficiency in **contract review and risk assessment**, helping users quickly identify key provisions.

For more details, visit [CUAD](https://www.atticusprojectai.org/cuad).

## Dataset Conversion for LLaMA Models

Since LLaMA models do not natively support direct ingestion of the CUAD dataset, the data has been **transformed into an optimized format**. The conversion process ensures compatibility and structured input handling for improved legal NLP performance.

- **Converted Dataset:** `alpaca_format_for_llama.json`
- **Conversion Code:** Implemented in `data_conversion.ipynb`
- **Source Dataset:** A subset of the **CUAD (Contract Understanding Atticus Dataset)**, containing **expert-annotated legal contract clauses**.

This adaptation enhances contract clause extraction and facilitates **efficient automated legal review** using large language models.
